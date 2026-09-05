# CreatePlanRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**name** | **str** |  | 
**monthly_docs** | **int** |  | [optional] [default to 0]
**max_rucs** | **int** |  | [optional] [default to 0]
**requests_per_minute** | **int** |  | [optional] [default to 0]
**allow_despatch** | **bool** |  | [optional] [default to True]
**price** | **float** |  | [optional] [default to 0]
**currency** | **str** |  | [optional] [default to 'PEN']
**sort_order** | **int** |  | [optional] [default to 0]
**is_active** | **bool** |  | [optional] [default to True]

## Example

```python
from intifact_sdk.models.create_plan_request import CreatePlanRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePlanRequest from a JSON string
create_plan_request_instance = CreatePlanRequest.from_json(json)
# print the JSON string representation of the object
print(CreatePlanRequest.to_json())

# convert the object into a dict
create_plan_request_dict = create_plan_request_instance.to_dict()
# create an instance of CreatePlanRequest from a dict
create_plan_request_from_dict = CreatePlanRequest.from_dict(create_plan_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


