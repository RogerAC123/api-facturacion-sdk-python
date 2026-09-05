# ListDocuments200ResponsePagination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **float** |  | 
**limit** | **float** |  | 
**total** | **float** |  | 
**total_pages** | **float** |  | 

## Example

```python
from intifact_sdk.models.list_documents200_response_pagination import ListDocuments200ResponsePagination

# TODO update the JSON string below
json = "{}"
# create an instance of ListDocuments200ResponsePagination from a JSON string
list_documents200_response_pagination_instance = ListDocuments200ResponsePagination.from_json(json)
# print the JSON string representation of the object
print(ListDocuments200ResponsePagination.to_json())

# convert the object into a dict
list_documents200_response_pagination_dict = list_documents200_response_pagination_instance.to_dict()
# create an instance of ListDocuments200ResponsePagination from a dict
list_documents200_response_pagination_from_dict = ListDocuments200ResponsePagination.from_dict(list_documents200_response_pagination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


