# SendInvoice202ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**estado** | **str** |  | 
**hash** | **str** |  | 
**signature_value** | **str** |  | 
**job_id** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.send_invoice202_response_data import SendInvoice202ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoice202ResponseData from a JSON string
send_invoice202_response_data_instance = SendInvoice202ResponseData.from_json(json)
# print the JSON string representation of the object
print(SendInvoice202ResponseData.to_json())

# convert the object into a dict
send_invoice202_response_data_dict = send_invoice202_response_data_instance.to_dict()
# create an instance of SendInvoice202ResponseData from a dict
send_invoice202_response_data_from_dict = SendInvoice202ResponseData.from_dict(send_invoice202_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


