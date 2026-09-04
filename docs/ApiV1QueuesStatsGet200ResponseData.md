# ApiV1QueuesStatsGet200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sunat_send** | **Dict[str, float]** |  | 
**sunat_summary** | **Dict[str, float]** |  | 
**sunat_ticket_poll** | **Dict[str, float]** |  | 
**sunat_gre_send** | **Dict[str, float]** |  | 
**sunat_gre_ticket_poll** | **Dict[str, float]** |  | 

## Example

```python
from intifact_sdk.models.api_v1_queues_stats_get200_response_data import ApiV1QueuesStatsGet200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1QueuesStatsGet200ResponseData from a JSON string
api_v1_queues_stats_get200_response_data_instance = ApiV1QueuesStatsGet200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ApiV1QueuesStatsGet200ResponseData.to_json())

# convert the object into a dict
api_v1_queues_stats_get200_response_data_dict = api_v1_queues_stats_get200_response_data_instance.to_dict()
# create an instance of ApiV1QueuesStatsGet200ResponseData from a dict
api_v1_queues_stats_get200_response_data_from_dict = ApiV1QueuesStatsGet200ResponseData.from_dict(api_v1_queues_stats_get200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


