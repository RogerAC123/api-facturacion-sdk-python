# ApiV1InvoiceSendPostRequestFormaPagoInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo** | **str** |  | 
**monto** | **float** |  | 
**cuota** | **int** |  | [optional] [default to 0]
**fecha_pago** | **str** |  | 

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post_request_forma_pago_inner import ApiV1InvoiceSendPostRequestFormaPagoInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPostRequestFormaPagoInner from a JSON string
api_v1_invoice_send_post_request_forma_pago_inner_instance = ApiV1InvoiceSendPostRequestFormaPagoInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPostRequestFormaPagoInner.to_json())

# convert the object into a dict
api_v1_invoice_send_post_request_forma_pago_inner_dict = api_v1_invoice_send_post_request_forma_pago_inner_instance.to_dict()
# create an instance of ApiV1InvoiceSendPostRequestFormaPagoInner from a dict
api_v1_invoice_send_post_request_forma_pago_inner_from_dict = ApiV1InvoiceSendPostRequestFormaPagoInner.from_dict(api_v1_invoice_send_post_request_forma_pago_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


