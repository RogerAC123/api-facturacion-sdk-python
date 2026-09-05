# SendVoidedRequestItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**motivo_baja** | **str** |  | 

## Example

```python
from intifact_sdk.models.send_voided_request_items_inner import SendVoidedRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendVoidedRequestItemsInner from a JSON string
send_voided_request_items_inner_instance = SendVoidedRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(SendVoidedRequestItemsInner.to_json())

# convert the object into a dict
send_voided_request_items_inner_dict = send_voided_request_items_inner_instance.to_dict()
# create an instance of SendVoidedRequestItemsInner from a dict
send_voided_request_items_inner_from_dict = SendVoidedRequestItemsInner.from_dict(send_voided_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


