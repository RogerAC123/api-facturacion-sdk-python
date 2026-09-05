# SendSummary202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**SendSummary202ResponseData**](SendSummary202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.send_summary202_response import SendSummary202Response

# TODO update the JSON string below
json = "{}"
# create an instance of SendSummary202Response from a JSON string
send_summary202_response_instance = SendSummary202Response.from_json(json)
# print the JSON string representation of the object
print(SendSummary202Response.to_json())

# convert the object into a dict
send_summary202_response_dict = send_summary202_response_instance.to_dict()
# create an instance of SendSummary202Response from a dict
send_summary202_response_from_dict = SendSummary202Response.from_dict(send_summary202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


