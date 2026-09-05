# ComputeInvoiceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_moneda** | **str** |  | [optional] [default to 'PEN']
**items** | [**List[ComputeInvoiceRequestItemsInner]**](ComputeInvoiceRequestItemsInner.md) |  | 
**descuento_global** | [**ComputeInvoiceRequestItemsInnerDescuento**](ComputeInvoiceRequestItemsInnerDescuento.md) |  | [optional] 
**precios_incluyen_igv** | **bool** |  | [optional] [default to False]

## Example

```python
from intifact_sdk.models.compute_invoice_request import ComputeInvoiceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ComputeInvoiceRequest from a JSON string
compute_invoice_request_instance = ComputeInvoiceRequest.from_json(json)
# print the JSON string representation of the object
print(ComputeInvoiceRequest.to_json())

# convert the object into a dict
compute_invoice_request_dict = compute_invoice_request_instance.to_dict()
# create an instance of ComputeInvoiceRequest from a dict
compute_invoice_request_from_dict = ComputeInvoiceRequest.from_dict(compute_invoice_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


