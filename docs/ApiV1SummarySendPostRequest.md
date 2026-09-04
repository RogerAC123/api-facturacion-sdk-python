# ApiV1SummarySendPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**correlativo** | **str** |  | 
**fecha_emision** | **str** |  | 
**fecha_referencia** | **str** |  | 
**items** | [**List[ApiV1SummarySendPostRequestItemsInner]**](ApiV1SummarySendPostRequestItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_summary_send_post_request import ApiV1SummarySendPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1SummarySendPostRequest from a JSON string
api_v1_summary_send_post_request_instance = ApiV1SummarySendPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1SummarySendPostRequest.to_json())

# convert the object into a dict
api_v1_summary_send_post_request_dict = api_v1_summary_send_post_request_instance.to_dict()
# create an instance of ApiV1SummarySendPostRequest from a dict
api_v1_summary_send_post_request_from_dict = ApiV1SummarySendPostRequest.from_dict(api_v1_summary_send_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


