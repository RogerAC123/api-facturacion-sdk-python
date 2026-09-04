# ApiV1CatalogsGet200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **str** |  | 
**name** | **str** |  | 
**items** | [**List[ApiV1CatalogsGet200ResponseDataInnerItemsInner]**](ApiV1CatalogsGet200ResponseDataInnerItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_catalogs_get200_response_data_inner import ApiV1CatalogsGet200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CatalogsGet200ResponseDataInner from a JSON string
api_v1_catalogs_get200_response_data_inner_instance = ApiV1CatalogsGet200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1CatalogsGet200ResponseDataInner.to_json())

# convert the object into a dict
api_v1_catalogs_get200_response_data_inner_dict = api_v1_catalogs_get200_response_data_inner_instance.to_dict()
# create an instance of ApiV1CatalogsGet200ResponseDataInner from a dict
api_v1_catalogs_get200_response_data_inner_from_dict = ApiV1CatalogsGet200ResponseDataInner.from_dict(api_v1_catalogs_get200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


