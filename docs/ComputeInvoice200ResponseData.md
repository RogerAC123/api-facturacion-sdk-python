# ComputeInvoice200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_moneda** | **str** |  | 
**items** | [**List[ComputeInvoice200ResponseDataItemsInner]**](ComputeInvoice200ResponseDataItemsInner.md) |  | 
**monto_oper_gravadas** | **float** |  | 
**monto_oper_exoneradas** | **float** |  | 
**monto_oper_inafectas** | **float** |  | 
**monto_oper_gratuitas** | **float** |  | 
**monto_oper_exportacion** | **float** |  | 
**monto_igv** | **float** |  | 
**monto_icbper** | **float** |  | 
**descuento_global** | **float** |  | 
**descuento_global_base** | **float** |  | 
**total_descuentos** | **float** |  | 
**total_impuestos** | **float** |  | 
**valor_venta** | **float** |  | 
**sub_total** | **float** |  | 
**monto_imp_venta** | **float** |  | 
**monto_en_letras** | **str** |  | 

## Example

```python
from intifact_sdk.models.compute_invoice200_response_data import ComputeInvoice200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ComputeInvoice200ResponseData from a JSON string
compute_invoice200_response_data_instance = ComputeInvoice200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ComputeInvoice200ResponseData.to_json())

# convert the object into a dict
compute_invoice200_response_data_dict = compute_invoice200_response_data_instance.to_dict()
# create an instance of ComputeInvoice200ResponseData from a dict
compute_invoice200_response_data_from_dict = ComputeInvoice200ResponseData.from_dict(compute_invoice200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


