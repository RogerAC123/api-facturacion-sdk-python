# ApiV1DocumentsGet200ResponsePagination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **float** |  | 
**limit** | **float** |  | 
**total** | **float** |  | 
**total_pages** | **float** |  | 

## Example

```python
from intifact_sdk.models.api_v1_documents_get200_response_pagination import ApiV1DocumentsGet200ResponsePagination

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DocumentsGet200ResponsePagination from a JSON string
api_v1_documents_get200_response_pagination_instance = ApiV1DocumentsGet200ResponsePagination.from_json(json)
# print the JSON string representation of the object
print(ApiV1DocumentsGet200ResponsePagination.to_json())

# convert the object into a dict
api_v1_documents_get200_response_pagination_dict = api_v1_documents_get200_response_pagination_instance.to_dict()
# create an instance of ApiV1DocumentsGet200ResponsePagination from a dict
api_v1_documents_get200_response_pagination_from_dict = ApiV1DocumentsGet200ResponsePagination.from_dict(api_v1_documents_get200_response_pagination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


