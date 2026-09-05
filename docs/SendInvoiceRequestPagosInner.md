# SendInvoiceRequestPagosInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metodo_pago** | **str** |  | 
**monto** | **float** |  | 

## Example

```python
from intifact_sdk.models.send_invoice_request_pagos_inner import SendInvoiceRequestPagosInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequestPagosInner from a JSON string
send_invoice_request_pagos_inner_instance = SendInvoiceRequestPagosInner.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequestPagosInner.to_json())

# convert the object into a dict
send_invoice_request_pagos_inner_dict = send_invoice_request_pagos_inner_instance.to_dict()
# create an instance of SendInvoiceRequestPagosInner from a dict
send_invoice_request_pagos_inner_from_dict = SendInvoiceRequestPagosInner.from_dict(send_invoice_request_pagos_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


