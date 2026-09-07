# SearchProductoSunat200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**SearchProductoSunat200ResponseData**](SearchProductoSunat200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.search_producto_sunat200_response import SearchProductoSunat200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SearchProductoSunat200Response from a JSON string
search_producto_sunat200_response_instance = SearchProductoSunat200Response.from_json(json)
# print the JSON string representation of the object
print(SearchProductoSunat200Response.to_json())

# convert the object into a dict
search_producto_sunat200_response_dict = search_producto_sunat200_response_instance.to_dict()
# create an instance of SearchProductoSunat200Response from a dict
search_producto_sunat200_response_from_dict = SearchProductoSunat200Response.from_dict(search_producto_sunat200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


