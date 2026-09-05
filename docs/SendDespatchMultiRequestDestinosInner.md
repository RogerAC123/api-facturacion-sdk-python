# SendDespatchMultiRequestDestinosInner


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
**detalle** | [**List[SendDespatchRequestDetalleInner]**](SendDespatchRequestDetalleInner.md) |  | 

## Example

```python
from intifact_sdk.models.send_despatch_multi_request_destinos_inner import SendDespatchMultiRequestDestinosInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchMultiRequestDestinosInner from a JSON string
send_despatch_multi_request_destinos_inner_instance = SendDespatchMultiRequestDestinosInner.from_json(json)
# print the JSON string representation of the object
print(SendDespatchMultiRequestDestinosInner.to_json())

# convert the object into a dict
send_despatch_multi_request_destinos_inner_dict = send_despatch_multi_request_destinos_inner_instance.to_dict()
# create an instance of SendDespatchMultiRequestDestinosInner from a dict
send_despatch_multi_request_destinos_inner_from_dict = SendDespatchMultiRequestDestinosInner.from_dict(send_despatch_multi_request_destinos_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


