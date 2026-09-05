# SendSummaryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**correlativo** | **str** |  | 
**fecha_emision** | **str** |  | 
**fecha_referencia** | **str** |  | 
**items** | [**List[SendSummaryRequestItemsInner]**](SendSummaryRequestItemsInner.md) |  | 

## Example

```python
from intifact_sdk.models.send_summary_request import SendSummaryRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendSummaryRequest from a JSON string
send_summary_request_instance = SendSummaryRequest.from_json(json)
# print the JSON string representation of the object
print(SendSummaryRequest.to_json())

# convert the object into a dict
send_summary_request_dict = send_summary_request_instance.to_dict()
# create an instance of SendSummaryRequest from a dict
send_summary_request_from_dict = SendSummaryRequest.from_dict(send_summary_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


