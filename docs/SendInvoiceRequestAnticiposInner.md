# SendInvoiceRequestAnticiposInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**nro_doc** | **str** |  | 
**total** | **float** |  | 
**valor** | **float** |  | 
**afectacion** | **str** |  | [optional] [default to '10']

## Example

```python
from intifact_sdk.models.send_invoice_request_anticipos_inner import SendInvoiceRequestAnticiposInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequestAnticiposInner from a JSON string
send_invoice_request_anticipos_inner_instance = SendInvoiceRequestAnticiposInner.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequestAnticiposInner.to_json())

# convert the object into a dict
send_invoice_request_anticipos_inner_dict = send_invoice_request_anticipos_inner_instance.to_dict()
# create an instance of SendInvoiceRequestAnticiposInner from a dict
send_invoice_request_anticipos_inner_from_dict = SendInvoiceRequestAnticiposInner.from_dict(send_invoice_request_anticipos_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


