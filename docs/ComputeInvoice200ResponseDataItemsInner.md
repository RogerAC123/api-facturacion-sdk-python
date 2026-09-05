# ComputeInvoice200ResponseDataItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unidad** | **str** |  | 
**cantidad** | **float** |  | 
**cod_producto** | **str** |  | 
**descripcion** | **str** |  | 
**marca** | **str** |  | [optional] 
**tip_afe_igv** | **str** |  | 
**porcentaje_igv** | **float** |  | 
**monto_valor_unitario** | **float** |  | 
**descuento** | **float** |  | 
**descuento_item** | **float** |  | 
**descuento_global_linea** | **float** |  | 
**monto_bruto** | **float** |  | 
**monto_valor_venta** | **float** |  | 
**monto_base_igv** | **float** |  | 
**igv** | **float** |  | 
**total_impuestos** | **float** |  | 
**monto_precio_unitario** | **float** |  | 
**factor_icbper** | **float** |  | 
**cod_prod_sunat** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.compute_invoice200_response_data_items_inner import ComputeInvoice200ResponseDataItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ComputeInvoice200ResponseDataItemsInner from a JSON string
compute_invoice200_response_data_items_inner_instance = ComputeInvoice200ResponseDataItemsInner.from_json(json)
# print the JSON string representation of the object
print(ComputeInvoice200ResponseDataItemsInner.to_json())

# convert the object into a dict
compute_invoice200_response_data_items_inner_dict = compute_invoice200_response_data_items_inner_instance.to_dict()
# create an instance of ComputeInvoice200ResponseDataItemsInner from a dict
compute_invoice200_response_data_items_inner_from_dict = ComputeInvoice200ResponseDataItemsInner.from_dict(compute_invoice200_response_data_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


