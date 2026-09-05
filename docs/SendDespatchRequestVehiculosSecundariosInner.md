# SendDespatchRequestVehiculosSecundariosInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**placa** | **str** |  | 
**tuc** | **str** |  | [optional] 
**autorizacion** | **str** |  | [optional] 
**autorizacion_entidad** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.send_despatch_request_vehiculos_secundarios_inner import SendDespatchRequestVehiculosSecundariosInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchRequestVehiculosSecundariosInner from a JSON string
send_despatch_request_vehiculos_secundarios_inner_instance = SendDespatchRequestVehiculosSecundariosInner.from_json(json)
# print the JSON string representation of the object
print(SendDespatchRequestVehiculosSecundariosInner.to_json())

# convert the object into a dict
send_despatch_request_vehiculos_secundarios_inner_dict = send_despatch_request_vehiculos_secundarios_inner_instance.to_dict()
# create an instance of SendDespatchRequestVehiculosSecundariosInner from a dict
send_despatch_request_vehiculos_secundarios_inner_from_dict = SendDespatchRequestVehiculosSecundariosInner.from_dict(send_despatch_request_vehiculos_secundarios_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


