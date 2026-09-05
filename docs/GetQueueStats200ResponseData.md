# GetQueueStats200ResponseData


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
from intifact_sdk.models.get_queue_stats200_response_data import GetQueueStats200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of GetQueueStats200ResponseData from a JSON string
get_queue_stats200_response_data_instance = GetQueueStats200ResponseData.from_json(json)
# print the JSON string representation of the object
print(GetQueueStats200ResponseData.to_json())

# convert the object into a dict
get_queue_stats200_response_data_dict = get_queue_stats200_response_data_instance.to_dict()
# create an instance of GetQueueStats200ResponseData from a dict
get_queue_stats200_response_data_from_dict = GetQueueStats200ResponseData.from_dict(get_queue_stats200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


