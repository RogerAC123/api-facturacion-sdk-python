# GetProductoSunat200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**ExportProductoSunat200ResponseDataItemsInner**](ExportProductoSunat200ResponseDataItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.get_producto_sunat200_response import GetProductoSunat200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetProductoSunat200Response from a JSON string
get_producto_sunat200_response_instance = GetProductoSunat200Response.from_json(json)
# print the JSON string representation of the object
print(GetProductoSunat200Response.to_json())

# convert the object into a dict
get_producto_sunat200_response_dict = get_producto_sunat200_response_instance.to_dict()
# create an instance of GetProductoSunat200Response from a dict
get_producto_sunat200_response_from_dict = GetProductoSunat200Response.from_dict(get_producto_sunat200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


