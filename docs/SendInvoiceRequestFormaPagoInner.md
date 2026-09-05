# SendInvoiceRequestFormaPagoInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo** | **str** |  | 
**monto** | **float** |  | 
**cuota** | **int** |  | [optional] [default to 0]
**fecha_pago** | **str** |  | 

## Example

```python
from intifact_sdk.models.send_invoice_request_forma_pago_inner import SendInvoiceRequestFormaPagoInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequestFormaPagoInner from a JSON string
send_invoice_request_forma_pago_inner_instance = SendInvoiceRequestFormaPagoInner.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequestFormaPagoInner.to_json())

# convert the object into a dict
send_invoice_request_forma_pago_inner_dict = send_invoice_request_forma_pago_inner_instance.to_dict()
# create an instance of SendInvoiceRequestFormaPagoInner from a dict
send_invoice_request_forma_pago_inner_from_dict = SendInvoiceRequestFormaPagoInner.from_dict(send_invoice_request_forma_pago_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


