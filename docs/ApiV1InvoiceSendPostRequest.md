# ApiV1InvoiceSendPostRequest


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
**detalle** | [**List[ApiV1InvoiceSendPostRequestDetalleInner]**](ApiV1InvoiceSendPostRequestDetalleInner.md) |  | 
**forma_pago** | [**List[ApiV1InvoiceSendPostRequestFormaPagoInner]**](ApiV1InvoiceSendPostRequestFormaPagoInner.md) |  | 
**leyendas** | [**List[ApiV1InvoiceSendPostRequestLeyendasInner]**](ApiV1InvoiceSendPostRequestLeyendasInner.md) |  | 
**observacion** | **str** |  | [optional] 
**vendedor** | **str** |  | [optional] 
**pagos** | [**List[ApiV1InvoiceSendPostRequestPagosInner]**](ApiV1InvoiceSendPostRequestPagosInner.md) |  | [optional] 
**detraccion** | [**ApiV1InvoiceSendPostRequestDetraccion**](ApiV1InvoiceSendPostRequestDetraccion.md) |  | [optional] 
**guia_remision** | [**List[ApiV1InvoiceSendPostRequestGuiaRemisionInner]**](ApiV1InvoiceSendPostRequestGuiaRemisionInner.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post_request import ApiV1InvoiceSendPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPostRequest from a JSON string
api_v1_invoice_send_post_request_instance = ApiV1InvoiceSendPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPostRequest.to_json())

# convert the object into a dict
api_v1_invoice_send_post_request_dict = api_v1_invoice_send_post_request_instance.to_dict()
# create an instance of ApiV1InvoiceSendPostRequest from a dict
api_v1_invoice_send_post_request_from_dict = ApiV1InvoiceSendPostRequest.from_dict(api_v1_invoice_send_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


