# ApiV1VoidedSendPostRequestItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**motivo_baja** | **str** |  | 

## Example

```python
from intifact_sdk.models.api_v1_voided_send_post_request_items_inner import ApiV1VoidedSendPostRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1VoidedSendPostRequestItemsInner from a JSON string
api_v1_voided_send_post_request_items_inner_instance = ApiV1VoidedSendPostRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1VoidedSendPostRequestItemsInner.to_json())

# convert the object into a dict
api_v1_voided_send_post_request_items_inner_dict = api_v1_voided_send_post_request_items_inner_instance.to_dict()
# create an instance of ApiV1VoidedSendPostRequestItemsInner from a dict
api_v1_voided_send_post_request_items_inner_from_dict = ApiV1VoidedSendPostRequestItemsInner.from_dict(api_v1_voided_send_post_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


