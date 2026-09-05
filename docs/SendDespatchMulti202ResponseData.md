# SendDespatchMulti202ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **float** |  | 
**emitidas** | **float** |  | 
**fallidas** | **float** |  | 
**guias** | [**List[SendDespatchMulti202ResponseDataGuiasInner]**](SendDespatchMulti202ResponseDataGuiasInner.md) |  | 

## Example

```python
from intifact_sdk.models.send_despatch_multi202_response_data import SendDespatchMulti202ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchMulti202ResponseData from a JSON string
send_despatch_multi202_response_data_instance = SendDespatchMulti202ResponseData.from_json(json)
# print the JSON string representation of the object
print(SendDespatchMulti202ResponseData.to_json())

# convert the object into a dict
send_despatch_multi202_response_data_dict = send_despatch_multi202_response_data_instance.to_dict()
# create an instance of SendDespatchMulti202ResponseData from a dict
send_despatch_multi202_response_data_from_dict = SendDespatchMulti202ResponseData.from_dict(send_despatch_multi202_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


