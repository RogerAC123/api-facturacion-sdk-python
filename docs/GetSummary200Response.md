# GetSummary200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**GetSummary200ResponseData**](GetSummary200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.get_summary200_response import GetSummary200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetSummary200Response from a JSON string
get_summary200_response_instance = GetSummary200Response.from_json(json)
# print the JSON string representation of the object
print(GetSummary200Response.to_json())

# convert the object into a dict
get_summary200_response_dict = get_summary200_response_instance.to_dict()
# create an instance of GetSummary200Response from a dict
get_summary200_response_from_dict = GetSummary200Response.from_dict(get_summary200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


