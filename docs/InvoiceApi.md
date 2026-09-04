# intifact_sdk.InvoiceApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_invoice_compute_post**](InvoiceApi.md#api_v1_invoice_compute_post) | **POST** /api/v1/invoice/compute | Calcular importes (IGV, descuentos, totales) sin emitir
[**api_v1_invoice_id_cdr_get**](InvoiceApi.md#api_v1_invoice_id_cdr_get) | **GET** /api/v1/invoice/{id}/cdr | Descargar CDR (constancia de SUNAT)
[**api_v1_invoice_id_pdf_get**](InvoiceApi.md#api_v1_invoice_id_pdf_get) | **GET** /api/v1/invoice/{id}/pdf | Obtener PDF (A4 oficina, ticket 80mm o ticket 58mm POS)
[**api_v1_invoice_id_xml_get**](InvoiceApi.md#api_v1_invoice_id_xml_get) | **GET** /api/v1/invoice/{id}/xml | Descargar XML firmado
[**api_v1_invoice_send_post**](InvoiceApi.md#api_v1_invoice_send_post) | **POST** /api/v1/invoice/send | Enviar factura (01) o boleta (03) a SUNAT


# **api_v1_invoice_compute_post**
> ApiV1InvoiceComputePost200Response api_v1_invoice_compute_post(api_v1_invoice_compute_post_request)

Calcular importes (IGV, descuentos, totales) sin emitir

Motor de cálculo: recibe ítems crudos (cantidad, valorUnitario sin IGV, afectación, descuento) y un descuento global opcional, y devuelve TODOS los importes fiscales calculados (bases, IGV, descuentos, totales, monto en letras). No emite ni persiste nada — úsalo para previsualizar o para alimentar POST /invoice/send.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_invoice_compute_post200_response import ApiV1InvoiceComputePost200Response
from intifact_sdk.models.api_v1_invoice_compute_post_request import ApiV1InvoiceComputePostRequest
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)


# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.InvoiceApi(api_client)
    api_v1_invoice_compute_post_request = intifact_sdk.ApiV1InvoiceComputePostRequest() # ApiV1InvoiceComputePostRequest | 

    try:
        # Calcular importes (IGV, descuentos, totales) sin emitir
        api_response = api_instance.api_v1_invoice_compute_post(api_v1_invoice_compute_post_request)
        print("The response of InvoiceApi->api_v1_invoice_compute_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceApi->api_v1_invoice_compute_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_invoice_compute_post_request** | [**ApiV1InvoiceComputePostRequest**](ApiV1InvoiceComputePostRequest.md)|  | 

### Return type

[**ApiV1InvoiceComputePost200Response**](ApiV1InvoiceComputePost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_invoice_id_cdr_get**
> api_v1_invoice_id_cdr_get(id)

Descargar CDR (constancia de SUNAT)

### Example


```python
import intifact_sdk
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)


# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.InvoiceApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar CDR (constancia de SUNAT)
        api_instance.api_v1_invoice_id_cdr_get(id)
    except Exception as e:
        print("Exception when calling InvoiceApi->api_v1_invoice_id_cdr_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_invoice_id_pdf_get**
> api_v1_invoice_id_pdf_get(id, format=format)

Obtener PDF (A4 oficina, ticket 80mm o ticket 58mm POS)

### Example


```python
import intifact_sdk
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)


# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.InvoiceApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    format = 'a4' # str |  (optional) (default to 'a4')

    try:
        # Obtener PDF (A4 oficina, ticket 80mm o ticket 58mm POS)
        api_instance.api_v1_invoice_id_pdf_get(id, format=format)
    except Exception as e:
        print("Exception when calling InvoiceApi->api_v1_invoice_id_pdf_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **format** | **str**|  | [optional] [default to &#39;a4&#39;]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_invoice_id_xml_get**
> api_v1_invoice_id_xml_get(id)

Descargar XML firmado

### Example


```python
import intifact_sdk
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)


# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.InvoiceApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar XML firmado
        api_instance.api_v1_invoice_id_xml_get(id)
    except Exception as e:
        print("Exception when calling InvoiceApi->api_v1_invoice_id_xml_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_invoice_send_post**
> ApiV1InvoiceSendPost202Response api_v1_invoice_send_post(api_v1_invoice_send_post_request)

Enviar factura (01) o boleta (03) a SUNAT

Genera el XML UBL 2.1, lo firma digitalmente y lo encola para envío asíncrono a SUNAT. Responde 202 inmediatamente. Para conocer el resultado final consultar GET /documents/{id}. Idempotente por (RUC emisor, tipoDoc, serie, correlativo): reenviar el mismo comprobante NO lo duplica. Si ya fue aceptado devuelve el mismo id y hash sin reenviar nada a SUNAT; si sigue en proceso responde 409 (esperá el resultado, no cambies el correlativo). Solo un RECHAZADO exige un correlativo nuevo.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_invoice_send_post202_response import ApiV1InvoiceSendPost202Response
from intifact_sdk.models.api_v1_invoice_send_post_request import ApiV1InvoiceSendPostRequest
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)


# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.InvoiceApi(api_client)
    api_v1_invoice_send_post_request = intifact_sdk.ApiV1InvoiceSendPostRequest() # ApiV1InvoiceSendPostRequest | 

    try:
        # Enviar factura (01) o boleta (03) a SUNAT
        api_response = api_instance.api_v1_invoice_send_post(api_v1_invoice_send_post_request)
        print("The response of InvoiceApi->api_v1_invoice_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceApi->api_v1_invoice_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_invoice_send_post_request** | [**ApiV1InvoiceSendPostRequest**](ApiV1InvoiceSendPostRequest.md)|  | 

### Return type

[**ApiV1InvoiceSendPost202Response**](ApiV1InvoiceSendPost202Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |
**409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

