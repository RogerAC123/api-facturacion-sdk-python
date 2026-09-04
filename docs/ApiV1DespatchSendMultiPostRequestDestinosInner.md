# ApiV1DespatchSendMultiPostRequestDestinosInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cliente_tipo_doc** | **str** |  | 
**cliente_num_doc** | **str** |  | 
**cliente_razon_social** | **str** |  | 
**cliente_direccion** | **str** |  | [optional] 
**cliente_distrito** | **str** |  | [optional] 
**cliente_provincia** | **str** |  | [optional] 
**cliente_departamento** | **str** |  | [optional] 
**destinatario_contacto** | **str** |  | [optional] 
**destinatario_telefono** | **str** |  | [optional] 
**destinatario_email** | **str** |  | [optional] 
**entrega_referencia** | **str** |  | [optional] 
**modalidad_entrega** | **str** |  | [optional] 
**agencia_nombre** | **str** |  | [optional] 
**agencia_sede** | **str** |  | [optional] 
**guia_llegada_ubigeo** | **str** |  | 
**guia_llegada_direccion** | **str** |  | 
**guia_peso_total** | **float** |  | 
**guia_und_peso_total** | **str** |  | [optional] [default to 'KGM']
**detalle** | [**List[ApiV1DespatchSendPostRequestDetalleInner]**](ApiV1DespatchSendPostRequestDetalleInner.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_despatch_send_multi_post_request_destinos_inner import ApiV1DespatchSendMultiPostRequestDestinosInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchSendMultiPostRequestDestinosInner from a JSON string
api_v1_despatch_send_multi_post_request_destinos_inner_instance = ApiV1DespatchSendMultiPostRequestDestinosInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchSendMultiPostRequestDestinosInner.to_json())

# convert the object into a dict
api_v1_despatch_send_multi_post_request_destinos_inner_dict = api_v1_despatch_send_multi_post_request_destinos_inner_instance.to_dict()
# create an instance of ApiV1DespatchSendMultiPostRequestDestinosInner from a dict
api_v1_despatch_send_multi_post_request_destinos_inner_from_dict = ApiV1DespatchSendMultiPostRequestDestinosInner.from_dict(api_v1_despatch_send_multi_post_request_destinos_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


