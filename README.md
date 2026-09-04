# intifact-sdk (Python)

SDK Python para la **API de Facturación Electrónica SUNAT de Intifact** (Perú),
generado con [OpenAPI Generator](https://openapi-generator.tech) desde el spec
que la API expone en `/docs/json`. Facturas, boletas, notas de crédito/débito,
guías de remisión (remitente y transportista), resúmenes diarios y
comunicaciones de baja.

## Requisitos

Python 3.10+

## Instalación

```bash
pip install intifact
```

## Autenticación

La API no está modelada con un `securityScheme` de OpenAPI (el chequeo de API
key vive en un plugin de Fastify), así que el header se agrega a mano — el
cliente lo manda en cada request a partir de ahí:

```python
import intifact_sdk
from intifact_sdk import ApiClient, Configuration

config = Configuration(host="https://api-facturacion.intifact.com")
client = ApiClient(config)
client.set_default_header("Authorization", f"Bearer {os.environ['FACTURACION_API_KEY']}")
```

## Uso básico — enviar una factura

```python
import os
from intifact_sdk import ApiClient, Configuration, ApiException
from intifact_sdk.api.invoice_api import InvoiceApi
from intifact_sdk.models.api_v1_invoice_send_post_request import ApiV1InvoiceSendPostRequest
from intifact_sdk.models.api_v1_invoice_send_post_request_detalle_inner import (
    ApiV1InvoiceSendPostRequestDetalleInner,
)

config = Configuration(host="https://api-facturacion.intifact.com")
with ApiClient(config) as client:
    client.set_default_header("Authorization", f"Bearer {os.environ['FACTURACION_API_KEY']}")
    invoice_api = InvoiceApi(client)

    item = ApiV1InvoiceSendPostRequestDetalleInner(
        unidad="NIU",
        cantidad=2,
        cod_producto="PROD001",
        descripcion="Laptop HP 15",
        monto_valor_unitario=2500.00,
        monto_base_igv=5000.00,
        porcentaje_igv=18,
        igv=900.00,
        tip_afe_igv="10",
        total_impuestos=900.00,
        monto_precio_unitario=2950.00,
        monto_valor_venta=5000.00,
        # Código de Producto SUNAT (UNSPSC) — SUNAT lo exige desde 2027-01-01
        # para determinados bienes (error 3496 si falta o es inválido).
        cod_prod_sunat="43211508",
    )

    body = ApiV1InvoiceSendPostRequest(
        empresa_ruc="20553510661",
        tipo_doc="01",
        serie="F001",
        correlativo="100",
        tipo_moneda="PEN",
        fecha_emision="2026-01-15",
        tipo_operacion="0101",
        cliente_tipo_doc="6",
        cliente_num_doc="20000000001",
        cliente_razon_social="EMPRESA CLIENTE SAC",
        detalle=[item],
        monto_oper_gravadas=5000.00,
        monto_oper_exoneradas=0,
        monto_igv=900.00,
        total_impuestos=900.00,
        valor_venta=5000.00,
        sub_total=5900.00,
        monto_imp_venta=5900.00,
        forma_pago=[{"tipo": "Contado", "monto": 5900.00, "fechaPago": "2026-01-15"}],
        leyendas=[{"legendCode": "1000", "legendValue": "CINCO MIL NOVECIENTOS CON 00/100 SOLES"}],
    )

    try:
        resp = invoice_api.api_v1_invoice_send_post(body)
        # 202 — el documento queda ENCOLADO, SUNAT lo procesa en background
        print("Encolado:", resp.data.id)
    except ApiException as e:
        # El body real del error (400/401/409/...) viene en e.body
        print(f"Error {e.status}: {e.body}")
```

Notas:
- Los campos usan `snake_case` en Python (`cod_producto`) aunque el JSON que
  viaja por HTTP sigue siendo `camelCase` (`codProducto`) — Pydantic hace la
  conversión con `alias` automáticamente.
- Pydantic valida los modelos **al construirlos**, antes de cualquier llamada
  de red: si falta un campo requerido (ej. `forma_pago`, `leyendas`), obtienes
  un `ValidationError` local en vez de esperar un 400 del servidor. Es una
  ventaja real del SDK Python frente a mandar un dict suelto.

## Manejo de errores

Toda respuesta fuera de 2xx llega como `ApiException` (no como excepción
genérica de red): `e.status` trae el código HTTP y `e.body` el JSON crudo
`{ success: false, message, errors? }` que devuelve la API.

```python
try:
    invoice_api.api_v1_invoice_send_post(body)
except ApiException as e:
    if e.status == 409:
        # Comprobante ya en proceso — NO reintentar con otro correlativo,
        # esperar el resultado. Ver /documents/{id} para el estado final.
        pass
```

## APIs disponibles

| Clase | Para qué |
|---|---|
| `InvoiceApi` | Facturas/boletas: enviar, PDF, XML, CDR |
| `NoteApi` | Notas de crédito/débito |
| `DespatchApi` | Guías de remisión (remitente y transportista) |
| `SummaryApi` | Resumen diario y comunicación de baja |
| `DocumentsApi` | Listar/consultar documentos, reintentar fallidos |
| `QueuesApi` | Estado de las colas BullMQ |
| `CompanyApi` / `BranchesApi` | Empresas y establecimientos (solo lectura) |
| `WebhooksApi` | Suscripciones y entregas de webhooks |
| `PlansApi` | Planes y consumo (quota) |
| `PublicApi` | Consulta pública de comprobantes (sin auth) |
| `AuthApi` | Autenticación |
| `SystemApi` | `/health`, catálogos SUNAT |

## Regenerar desde la API

El proyecto se generó con [OpenAPI Generator](https://openapi-generator.tech)
(`python`) contra `https://api-facturacion.intifact.com/docs/json`. Para
regenerar tras un cambio de la API:

```bash
npx @openapitools/openapi-generator-cli generate \
  -i https://api-facturacion.intifact.com/docs/json \
  -g python --package-name intifact_sdk \
  -o .
```

## Nota sobre los nombres de métodos

Las rutas de la API no declaran `operationId` explícito en su schema de
Fastify, así que el generador deriva nombres desde el método+path
(`api_v1_invoice_send_post` en vez de algo como `send_invoice`). Si la API le
agrega `operationId` a sus rutas, una regeneración futura produciría nombres
más limpios sin romper compatibilidad de comportamiento.
