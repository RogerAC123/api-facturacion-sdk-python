# GetSummary200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**env** | **str** |  | 
**tipo** | **str** |  | 
**correlativo** | **str** |  | 
**fecha_emision** | **str** |  | 
**fecha_referencia** | **str** |  | 
**estado** | **str** |  | 
**ticket** | **str** |  | 
**codigo_respuesta** | **str** |  | 
**descripcion_respuesta** | **str** |  | 
**ultimo_error** | **str** |  | 
**intentos** | **float** |  | 
**tiene_cdr** | **bool** |  | 
**items** | [**List[GetSummary200ResponseDataItemsInner]**](GetSummary200ResponseDataItemsInner.md) |  | 
**created_at** | **str** |  | 

## Example

```python
from intifact_sdk.models.get_summary200_response_data import GetSummary200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of GetSummary200ResponseData from a JSON string
get_summary200_response_data_instance = GetSummary200ResponseData.from_json(json)
# print the JSON string representation of the object
print(GetSummary200ResponseData.to_json())

# convert the object into a dict
get_summary200_response_data_dict = get_summary200_response_data_instance.to_dict()
# create an instance of GetSummary200ResponseData from a dict
get_summary200_response_data_from_dict = GetSummary200ResponseData.from_dict(get_summary200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


