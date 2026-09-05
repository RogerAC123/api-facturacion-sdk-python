# SendDespatchMulti202ResponseDataGuiasInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**code** | **str** |  | [optional] 
**destino** | **float** |  | 
**data** | [**SendInvoice202ResponseData**](SendInvoice202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.send_despatch_multi202_response_data_guias_inner import SendDespatchMulti202ResponseDataGuiasInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchMulti202ResponseDataGuiasInner from a JSON string
send_despatch_multi202_response_data_guias_inner_instance = SendDespatchMulti202ResponseDataGuiasInner.from_json(json)
# print the JSON string representation of the object
print(SendDespatchMulti202ResponseDataGuiasInner.to_json())

# convert the object into a dict
send_despatch_multi202_response_data_guias_inner_dict = send_despatch_multi202_response_data_guias_inner_instance.to_dict()
# create an instance of SendDespatchMulti202ResponseDataGuiasInner from a dict
send_despatch_multi202_response_data_guias_inner_from_dict = SendDespatchMulti202ResponseDataGuiasInner.from_dict(send_despatch_multi202_response_data_guias_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


