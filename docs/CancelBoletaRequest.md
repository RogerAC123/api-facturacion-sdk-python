# CancelBoletaRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**motivo_baja** | **str** |  | 
**rc_correlativo** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.cancel_boleta_request import CancelBoletaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CancelBoletaRequest from a JSON string
cancel_boleta_request_instance = CancelBoletaRequest.from_json(json)
# print the JSON string representation of the object
print(CancelBoletaRequest.to_json())

# convert the object into a dict
cancel_boleta_request_dict = cancel_boleta_request_instance.to_dict()
# create an instance of CancelBoletaRequest from a dict
cancel_boleta_request_from_dict = CancelBoletaRequest.from_dict(cancel_boleta_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


