# ApiV1PlansPostRequest


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
from intifact_sdk.models.api_v1_plans_post_request import ApiV1PlansPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1PlansPostRequest from a JSON string
api_v1_plans_post_request_instance = ApiV1PlansPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1PlansPostRequest.to_json())

# convert the object into a dict
api_v1_plans_post_request_dict = api_v1_plans_post_request_instance.to_dict()
# create an instance of ApiV1PlansPostRequest from a dict
api_v1_plans_post_request_from_dict = ApiV1PlansPostRequest.from_dict(api_v1_plans_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


