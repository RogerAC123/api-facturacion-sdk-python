# ApiV1InvoiceSendPost202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**ApiV1InvoiceSendPost202ResponseData**](ApiV1InvoiceSendPost202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post202_response import ApiV1InvoiceSendPost202Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPost202Response from a JSON string
api_v1_invoice_send_post202_response_instance = ApiV1InvoiceSendPost202Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPost202Response.to_json())

# convert the object into a dict
api_v1_invoice_send_post202_response_dict = api_v1_invoice_send_post202_response_instance.to_dict()
# create an instance of ApiV1InvoiceSendPost202Response from a dict
api_v1_invoice_send_post202_response_from_dict = ApiV1InvoiceSendPost202Response.from_dict(api_v1_invoice_send_post202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


