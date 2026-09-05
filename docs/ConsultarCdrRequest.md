# ConsultarCdrRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ruc** | **str** |  | 
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**numero** | **str** |  | 

## Example

```python
from intifact_sdk.models.consultar_cdr_request import ConsultarCdrRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConsultarCdrRequest from a JSON string
consultar_cdr_request_instance = ConsultarCdrRequest.from_json(json)
# print the JSON string representation of the object
print(ConsultarCdrRequest.to_json())

# convert the object into a dict
consultar_cdr_request_dict = consultar_cdr_request_instance.to_dict()
# create an instance of ConsultarCdrRequest from a dict
consultar_cdr_request_from_dict = ConsultarCdrRequest.from_dict(consultar_cdr_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


