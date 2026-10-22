# GetSummary200ResponseDataItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**document_id** | **str** |  | 
**estado_documento** | **str** |  | 

## Example

```python
from intifact_sdk.models.get_summary200_response_data_items_inner import GetSummary200ResponseDataItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetSummary200ResponseDataItemsInner from a JSON string
get_summary200_response_data_items_inner_instance = GetSummary200ResponseDataItemsInner.from_json(json)
# print the JSON string representation of the object
print(GetSummary200ResponseDataItemsInner.to_json())

# convert the object into a dict
get_summary200_response_data_items_inner_dict = get_summary200_response_data_items_inner_instance.to_dict()
# create an instance of GetSummary200ResponseDataItemsInner from a dict
get_summary200_response_data_items_inner_from_dict = GetSummary200ResponseDataItemsInner.from_dict(get_summary200_response_data_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


