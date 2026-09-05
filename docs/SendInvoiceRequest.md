# SendInvoiceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_operacion** | **str** |  | [optional] [default to '0101']
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**tipo_moneda** | **str** |  | [optional] [default to 'PEN']
**fecha_emision** | **str** |  | 
**empresa_ruc** | **str** |  | 
**establecimiento_codigo** | **str** |  | [optional] [default to '0000']
**cliente_tipo_doc** | **str** |  | 
**cliente_num_doc** | **str** |  | 
**cliente_razon_social** | **str** |  | 
**cliente_direccion** | **str** |  | [optional] 
**cliente_distrito** | **str** |  | [optional] 
**cliente_provincia** | **str** |  | [optional] 
**cliente_departamento** | **str** |  | [optional] 
**monto_oper_gravadas** | **float** |  | [optional] [default to 0]
**monto_oper_exoneradas** | **float** |  | [optional] [default to 0]
**monto_oper_inafectas** | **float** |  | [optional] [default to 0]
**monto_oper_gratuitas** | **float** |  | [optional] [default to 0]
**monto_igv** | **float** |  | 
**total_impuestos** | **float** |  | 
**valor_venta** | **float** |  | 
**sub_total** | **float** |  | 
**monto_imp_venta** | **float** |  | 
**descuento_global** | **float** |  | [optional] 
**descuento_global_base** | **float** |  | [optional] 
**detalle** | [**List[SendInvoiceRequestDetalleInner]**](SendInvoiceRequestDetalleInner.md) |  | 
**forma_pago** | [**List[SendInvoiceRequestFormaPagoInner]**](SendInvoiceRequestFormaPagoInner.md) |  | 
**leyendas** | [**List[SendInvoiceRequestLeyendasInner]**](SendInvoiceRequestLeyendasInner.md) |  | 
**observacion** | **str** |  | [optional] 
**vendedor** | **str** |  | [optional] 
**pagos** | [**List[SendInvoiceRequestPagosInner]**](SendInvoiceRequestPagosInner.md) |  | [optional] 
**detraccion** | [**SendInvoiceRequestDetraccion**](SendInvoiceRequestDetraccion.md) |  | [optional] 
**guia_remision** | [**List[SendInvoiceRequestGuiaRemisionInner]**](SendInvoiceRequestGuiaRemisionInner.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.send_invoice_request import SendInvoiceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequest from a JSON string
send_invoice_request_instance = SendInvoiceRequest.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequest.to_json())

# convert the object into a dict
send_invoice_request_dict = send_invoice_request_instance.to_dict()
# create an instance of SendInvoiceRequest from a dict
send_invoice_request_from_dict = SendInvoiceRequest.from_dict(send_invoice_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


