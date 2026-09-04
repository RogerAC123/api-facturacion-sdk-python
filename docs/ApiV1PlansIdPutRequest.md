# ApiV1PlansIdPutRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**monthly_docs** | **int** |  | [optional] 
**max_rucs** | **int** |  | [optional] 
**requests_per_minute** | **int** |  | [optional] 
**allow_despatch** | **bool** |  | [optional] 
**price** | **float** |  | [optional] 
**currency** | **str** |  | [optional] 
**sort_order** | **int** |  | [optional] 
**is_active** | **bool** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_plans_id_put_request import ApiV1PlansIdPutRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1PlansIdPutRequest from a JSON string
api_v1_plans_id_put_request_instance = ApiV1PlansIdPutRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1PlansIdPutRequest.to_json())

# convert the object into a dict
api_v1_plans_id_put_request_dict = api_v1_plans_id_put_request_instance.to_dict()
# create an instance of ApiV1PlansIdPutRequest from a dict
api_v1_plans_id_put_request_from_dict = ApiV1PlansIdPutRequest.from_dict(api_v1_plans_id_put_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


