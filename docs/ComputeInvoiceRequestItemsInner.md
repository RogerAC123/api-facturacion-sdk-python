# ComputeInvoiceRequestItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**descripcion** | **str** |  | 
**cantidad** | **float** |  | 
**valor_unitario** | **float** |  | 
**unidad** | **str** |  | [optional] 
**cod_producto** | **str** |  | [optional] 
**afectacion** | **str** |  | [optional] [default to '10']
**igv_porcentaje** | **float** |  | [optional] [default to 18]
**descuento** | [**ComputeInvoiceRequestItemsInnerDescuento**](ComputeInvoiceRequestItemsInnerDescuento.md) |  | [optional] 
**factor_icbper** | **float** |  | [optional] [default to 0]
**marca** | **str** |  | [optional] 
**cod_prod_sunat** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.compute_invoice_request_items_inner import ComputeInvoiceRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ComputeInvoiceRequestItemsInner from a JSON string
compute_invoice_request_items_inner_instance = ComputeInvoiceRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(ComputeInvoiceRequestItemsInner.to_json())

# convert the object into a dict
compute_invoice_request_items_inner_dict = compute_invoice_request_items_inner_instance.to_dict()
# create an instance of ComputeInvoiceRequestItemsInner from a dict
compute_invoice_request_items_inner_from_dict = ComputeInvoiceRequestItemsInner.from_dict(compute_invoice_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


