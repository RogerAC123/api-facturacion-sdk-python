# SendDespatchRequestIndicadores


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
from intifact_sdk.models.send_despatch_request_indicadores import SendDespatchRequestIndicadores

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchRequestIndicadores from a JSON string
send_despatch_request_indicadores_instance = SendDespatchRequestIndicadores.from_json(json)
# print the JSON string representation of the object
print(SendDespatchRequestIndicadores.to_json())

# convert the object into a dict
send_despatch_request_indicadores_dict = send_despatch_request_indicadores_instance.to_dict()
# create an instance of SendDespatchRequestIndicadores from a dict
send_despatch_request_indicadores_from_dict = SendDespatchRequestIndicadores.from_dict(send_despatch_request_indicadores_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


