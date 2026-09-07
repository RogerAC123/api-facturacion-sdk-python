# ExportProductoSunat200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | 
**total** | **float** |  | 
**items** | [**List[ExportProductoSunat200ResponseDataItemsInner]**](ExportProductoSunat200ResponseDataItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.export_producto_sunat200_response_data import ExportProductoSunat200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ExportProductoSunat200ResponseData from a JSON string
export_producto_sunat200_response_data_instance = ExportProductoSunat200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ExportProductoSunat200ResponseData.to_json())

# convert the object into a dict
export_producto_sunat200_response_data_dict = export_producto_sunat200_response_data_instance.to_dict()
# create an instance of ExportProductoSunat200ResponseData from a dict
export_producto_sunat200_response_data_from_dict = ExportProductoSunat200ResponseData.from_dict(export_producto_sunat200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


