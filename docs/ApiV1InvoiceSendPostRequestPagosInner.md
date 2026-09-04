# ApiV1InvoiceSendPostRequestPagosInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metodo_pago** | **str** |  | 
**monto** | **float** |  | 

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post_request_pagos_inner import ApiV1InvoiceSendPostRequestPagosInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPostRequestPagosInner from a JSON string
api_v1_invoice_send_post_request_pagos_inner_instance = ApiV1InvoiceSendPostRequestPagosInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPostRequestPagosInner.to_json())

# convert the object into a dict
api_v1_invoice_send_post_request_pagos_inner_dict = api_v1_invoice_send_post_request_pagos_inner_instance.to_dict()
# create an instance of ApiV1InvoiceSendPostRequestPagosInner from a dict
api_v1_invoice_send_post_request_pagos_inner_from_dict = ApiV1InvoiceSendPostRequestPagosInner.from_dict(api_v1_invoice_send_post_request_pagos_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


