# SendVoidedRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**correlativo** | **str** |  | 
**fecha_emision** | **str** |  | 
**fecha_referencia** | **str** |  | 
**items** | [**List[SendVoidedRequestItemsInner]**](SendVoidedRequestItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.send_voided_request import SendVoidedRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendVoidedRequest from a JSON string
send_voided_request_instance = SendVoidedRequest.from_json(json)
# print the JSON string representation of the object
print(SendVoidedRequest.to_json())

# convert the object into a dict
send_voided_request_dict = send_voided_request_instance.to_dict()
# create an instance of SendVoidedRequest from a dict
send_voided_request_from_dict = SendVoidedRequest.from_dict(send_voided_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


