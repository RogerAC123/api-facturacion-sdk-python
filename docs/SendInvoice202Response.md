# SendInvoice202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**SendInvoice202ResponseData**](SendInvoice202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.send_invoice202_response import SendInvoice202Response

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoice202Response from a JSON string
send_invoice202_response_instance = SendInvoice202Response.from_json(json)
# print the JSON string representation of the object
print(SendInvoice202Response.to_json())

# convert the object into a dict
send_invoice202_response_dict = send_invoice202_response_instance.to_dict()
# create an instance of SendInvoice202Response from a dict
send_invoice202_response_from_dict = SendInvoice202Response.from_dict(send_invoice202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


