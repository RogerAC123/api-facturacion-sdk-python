# ListCatalogs200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**List[ListCatalogs200ResponseDataInner]**](ListCatalogs200ResponseDataInner.md) |  | 

## Example

```python
from intifact_sdk.models.list_catalogs200_response import ListCatalogs200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListCatalogs200Response from a JSON string
list_catalogs200_response_instance = ListCatalogs200Response.from_json(json)
# print the JSON string representation of the object
print(ListCatalogs200Response.to_json())

# convert the object into a dict
list_catalogs200_response_dict = list_catalogs200_response_instance.to_dict()
# create an instance of ListCatalogs200Response from a dict
list_catalogs200_response_from_dict = ListCatalogs200Response.from_dict(list_catalogs200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


