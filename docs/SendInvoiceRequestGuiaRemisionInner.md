# SendInvoiceRequestGuiaRemisionInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | [optional] [default to '09']
**nro_doc** | **str** |  | 

## Example

```python
from intifact_sdk.models.send_invoice_request_guia_remision_inner import SendInvoiceRequestGuiaRemisionInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequestGuiaRemisionInner from a JSON string
send_invoice_request_guia_remision_inner_instance = SendInvoiceRequestGuiaRemisionInner.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequestGuiaRemisionInner.to_json())

# convert the object into a dict
send_invoice_request_guia_remision_inner_dict = send_invoice_request_guia_remision_inner_instance.to_dict()
# create an instance of SendInvoiceRequestGuiaRemisionInner from a dict
send_invoice_request_guia_remision_inner_from_dict = SendInvoiceRequestGuiaRemisionInner.from_dict(send_invoice_request_guia_remision_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


