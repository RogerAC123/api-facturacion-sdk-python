# ApiV1InvoiceComputePost200ResponseDataItemsInner


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
from intifact_sdk.models.api_v1_invoice_compute_post200_response_data_items_inner import ApiV1InvoiceComputePost200ResponseDataItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceComputePost200ResponseDataItemsInner from a JSON string
api_v1_invoice_compute_post200_response_data_items_inner_instance = ApiV1InvoiceComputePost200ResponseDataItemsInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceComputePost200ResponseDataItemsInner.to_json())

# convert the object into a dict
api_v1_invoice_compute_post200_response_data_items_inner_dict = api_v1_invoice_compute_post200_response_data_items_inner_instance.to_dict()
# create an instance of ApiV1InvoiceComputePost200ResponseDataItemsInner from a dict
api_v1_invoice_compute_post200_response_data_items_inner_from_dict = ApiV1InvoiceComputePost200ResponseDataItemsInner.from_dict(api_v1_invoice_compute_post200_response_data_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


