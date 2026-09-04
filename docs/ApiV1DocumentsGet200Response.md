# ApiV1DocumentsGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**List[ApiV1DocumentsGet200ResponseDataInner]**](ApiV1DocumentsGet200ResponseDataInner.md) |  | 
**pagination** | [**ApiV1DocumentsGet200ResponsePagination**](ApiV1DocumentsGet200ResponsePagination.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_documents_get200_response import ApiV1DocumentsGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DocumentsGet200Response from a JSON string
api_v1_documents_get200_response_instance = ApiV1DocumentsGet200Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1DocumentsGet200Response.to_json())

# convert the object into a dict
api_v1_documents_get200_response_dict = api_v1_documents_get200_response_instance.to_dict()
# create an instance of ApiV1DocumentsGet200Response from a dict
api_v1_documents_get200_response_from_dict = ApiV1DocumentsGet200Response.from_dict(api_v1_documents_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


