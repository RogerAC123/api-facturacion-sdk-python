# ApiV1DespatchSendPostRequestIndicadores


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**transbordo_programado** | **bool** |  | [optional] 
**vehiculo_m1_l** | **bool** |  | [optional] 
**retorno_vehiculo_envase_vacio** | **bool** |  | [optional] 
**retorno_vehiculo_vacio** | **bool** |  | [optional] 
**traslado_total_dam_ds** | **bool** |  | [optional] 
**registro_transportista** | **bool** |  | [optional] 
**traslado_contenedor_manifiesto** | **bool** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_despatch_send_post_request_indicadores import ApiV1DespatchSendPostRequestIndicadores

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchSendPostRequestIndicadores from a JSON string
api_v1_despatch_send_post_request_indicadores_instance = ApiV1DespatchSendPostRequestIndicadores.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchSendPostRequestIndicadores.to_json())

# convert the object into a dict
api_v1_despatch_send_post_request_indicadores_dict = api_v1_despatch_send_post_request_indicadores_instance.to_dict()
# create an instance of ApiV1DespatchSendPostRequestIndicadores from a dict
api_v1_despatch_send_post_request_indicadores_from_dict = ApiV1DespatchSendPostRequestIndicadores.from_dict(api_v1_despatch_send_post_request_indicadores_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


