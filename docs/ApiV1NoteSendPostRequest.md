# ApiV1NoteSendPostRequest


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
**afectado_tipo_doc** | **str** |  | 
**afectado_num_doc** | **str** |  | 
**motivo_cod** | **str** |  | 
**motivo_des** | **str** |  | 
**monto_oper_gravadas** | **float** |  | [optional] [default to 0]
**monto_oper_exoneradas** | **float** |  | [optional] [default to 0]
**monto_oper_inafectas** | **float** |  | [optional] [default to 0]
**monto_igv** | **float** |  | 
**total_impuestos** | **float** |  | 
**valor_venta** | **float** |  | 
**sub_total** | **float** |  | 
**monto_imp_venta** | **float** |  | 
**descuento_global** | **float** |  | [optional] 
**descuento_global_base** | **float** |  | [optional] 
**detalle** | [**List[ApiV1NoteSendPostRequestDetalleInner]**](ApiV1NoteSendPostRequestDetalleInner.md) |  | 
**leyendas** | [**List[ApiV1InvoiceSendPostRequestLeyendasInner]**](ApiV1InvoiceSendPostRequestLeyendasInner.md) |  | 
**observacion** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_note_send_post_request import ApiV1NoteSendPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1NoteSendPostRequest from a JSON string
api_v1_note_send_post_request_instance = ApiV1NoteSendPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1NoteSendPostRequest.to_json())

# convert the object into a dict
api_v1_note_send_post_request_dict = api_v1_note_send_post_request_instance.to_dict()
# create an instance of ApiV1NoteSendPostRequest from a dict
api_v1_note_send_post_request_from_dict = ApiV1NoteSendPostRequest.from_dict(api_v1_note_send_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


