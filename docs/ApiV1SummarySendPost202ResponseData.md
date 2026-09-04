# ApiV1SummarySendPost202ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**estado** | **str** |  | [optional] 
**ticket** | **str** |  | [optional] 
**hash** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_summary_send_post202_response_data import ApiV1SummarySendPost202ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1SummarySendPost202ResponseData from a JSON string
api_v1_summary_send_post202_response_data_instance = ApiV1SummarySendPost202ResponseData.from_json(json)
# print the JSON string representation of the object
print(ApiV1SummarySendPost202ResponseData.to_json())

# convert the object into a dict
api_v1_summary_send_post202_response_data_dict = api_v1_summary_send_post202_response_data_instance.to_dict()
# create an instance of ApiV1SummarySendPost202ResponseData from a dict
api_v1_summary_send_post202_response_data_from_dict = ApiV1SummarySendPost202ResponseData.from_dict(api_v1_summary_send_post202_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


