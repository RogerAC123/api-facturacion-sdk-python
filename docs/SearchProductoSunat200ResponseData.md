# SearchProductoSunat200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | 
**q** | **str** |  | 
**total** | **float** |  | 
**items** | [**List[ExportProductoSunat200ResponseDataItemsInner]**](ExportProductoSunat200ResponseDataItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.search_producto_sunat200_response_data import SearchProductoSunat200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of SearchProductoSunat200ResponseData from a JSON string
search_producto_sunat200_response_data_instance = SearchProductoSunat200ResponseData.from_json(json)
# print the JSON string representation of the object
print(SearchProductoSunat200ResponseData.to_json())

# convert the object into a dict
search_producto_sunat200_response_data_dict = search_producto_sunat200_response_data_instance.to_dict()
# create an instance of SearchProductoSunat200ResponseData from a dict
search_producto_sunat200_response_data_from_dict = SearchProductoSunat200ResponseData.from_dict(search_producto_sunat200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


