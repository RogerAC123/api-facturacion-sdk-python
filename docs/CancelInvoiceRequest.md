# CancelInvoiceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**motivo_baja** | **str** |  | 
**ra_correlativo** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.cancel_invoice_request import CancelInvoiceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CancelInvoiceRequest from a JSON string
cancel_invoice_request_instance = CancelInvoiceRequest.from_json(json)
# print the JSON string representation of the object
print(CancelInvoiceRequest.to_json())

# convert the object into a dict
cancel_invoice_request_dict = cancel_invoice_request_instance.to_dict()
# create an instance of CancelInvoiceRequest from a dict
cancel_invoice_request_from_dict = CancelInvoiceRequest.from_dict(cancel_invoice_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


