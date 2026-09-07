# ExportProductoSunat200ResponseDataItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**codigo** | **str** |  | 
**descripcion** | **str** |  | 
**nivel** | **str** |  | 
**clase_codigo** | **str** |  | 
**familia** | **str** |  | 
**segmento** | **str** |  | 

## Example

```python
from intifact_sdk.models.export_producto_sunat200_response_data_items_inner import ExportProductoSunat200ResponseDataItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ExportProductoSunat200ResponseDataItemsInner from a JSON string
export_producto_sunat200_response_data_items_inner_instance = ExportProductoSunat200ResponseDataItemsInner.from_json(json)
# print the JSON string representation of the object
print(ExportProductoSunat200ResponseDataItemsInner.to_json())

# convert the object into a dict
export_producto_sunat200_response_data_items_inner_dict = export_producto_sunat200_response_data_items_inner_instance.to_dict()
# create an instance of ExportProductoSunat200ResponseDataItemsInner from a dict
export_producto_sunat200_response_data_items_inner_from_dict = ExportProductoSunat200ResponseDataItemsInner.from_dict(export_producto_sunat200_response_data_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


