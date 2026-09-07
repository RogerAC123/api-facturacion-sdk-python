# ExportProductoSunat200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**ExportProductoSunat200ResponseData**](ExportProductoSunat200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.export_producto_sunat200_response import ExportProductoSunat200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ExportProductoSunat200Response from a JSON string
export_producto_sunat200_response_instance = ExportProductoSunat200Response.from_json(json)
# print the JSON string representation of the object
print(ExportProductoSunat200Response.to_json())

# convert the object into a dict
export_producto_sunat200_response_dict = export_producto_sunat200_response_instance.to_dict()
# create an instance of ExportProductoSunat200Response from a dict
export_producto_sunat200_response_from_dict = ExportProductoSunat200Response.from_dict(export_producto_sunat200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


