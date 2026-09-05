# GetQueueStats200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**GetQueueStats200ResponseData**](GetQueueStats200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.get_queue_stats200_response import GetQueueStats200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetQueueStats200Response from a JSON string
get_queue_stats200_response_instance = GetQueueStats200Response.from_json(json)
# print the JSON string representation of the object
print(GetQueueStats200Response.to_json())

# convert the object into a dict
get_queue_stats200_response_dict = get_queue_stats200_response_instance.to_dict()
# create an instance of GetQueueStats200Response from a dict
get_queue_stats200_response_from_dict = GetQueueStats200Response.from_dict(get_queue_stats200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


