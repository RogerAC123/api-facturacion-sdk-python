# SendSummary202ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**estado** | **str** |  | [optional] 
**ticket** | **str** |  | [optional] 
**hash** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.send_summary202_response_data import SendSummary202ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of SendSummary202ResponseData from a JSON string
send_summary202_response_data_instance = SendSummary202ResponseData.from_json(json)
# print the JSON string representation of the object
print(SendSummary202ResponseData.to_json())

# convert the object into a dict
send_summary202_response_data_dict = send_summary202_response_data_instance.to_dict()
# create an instance of SendSummary202ResponseData from a dict
send_summary202_response_data_from_dict = SendSummary202ResponseData.from_dict(send_summary202_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


