# ApiV1VoidedSendPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**correlativo** | **str** |  | 
**fecha_emision** | **str** |  | 
**fecha_referencia** | **str** |  | 
**items** | [**List[ApiV1VoidedSendPostRequestItemsInner]**](ApiV1VoidedSendPostRequestItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_voided_send_post_request import ApiV1VoidedSendPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1VoidedSendPostRequest from a JSON string
api_v1_voided_send_post_request_instance = ApiV1VoidedSendPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1VoidedSendPostRequest.to_json())

# convert the object into a dict
api_v1_voided_send_post_request_dict = api_v1_voided_send_post_request_instance.to_dict()
# create an instance of ApiV1VoidedSendPostRequest from a dict
api_v1_voided_send_post_request_from_dict = ApiV1VoidedSendPostRequest.from_dict(api_v1_voided_send_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


