# GetNextCorrelativo200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**data** | [**GetNextCorrelativo200ResponseData**](GetNextCorrelativo200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.get_next_correlativo200_response import GetNextCorrelativo200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetNextCorrelativo200Response from a JSON string
get_next_correlativo200_response_instance = GetNextCorrelativo200Response.from_json(json)
# print the JSON string representation of the object
print(GetNextCorrelativo200Response.to_json())

# convert the object into a dict
get_next_correlativo200_response_dict = get_next_correlativo200_response_instance.to_dict()
# create an instance of GetNextCorrelativo200Response from a dict
get_next_correlativo200_response_from_dict = GetNextCorrelativo200Response.from_dict(get_next_correlativo200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


