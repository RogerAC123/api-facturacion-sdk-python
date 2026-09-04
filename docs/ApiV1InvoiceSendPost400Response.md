# ApiV1InvoiceSendPost400Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**code** | **str** |  | [optional] 
**errors** | [**List[ApiV1InvoiceSendPost400ResponseErrorsInner]**](ApiV1InvoiceSendPost400ResponseErrorsInner.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post400_response import ApiV1InvoiceSendPost400Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPost400Response from a JSON string
api_v1_invoice_send_post400_response_instance = ApiV1InvoiceSendPost400Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPost400Response.to_json())

# convert the object into a dict
api_v1_invoice_send_post400_response_dict = api_v1_invoice_send_post400_response_instance.to_dict()
# create an instance of ApiV1InvoiceSendPost400Response from a dict
api_v1_invoice_send_post400_response_from_dict = ApiV1InvoiceSendPost400Response.from_dict(api_v1_invoice_send_post400_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


