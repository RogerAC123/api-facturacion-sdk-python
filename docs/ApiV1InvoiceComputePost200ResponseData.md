# ApiV1InvoiceComputePost200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_moneda** | **str** |  | 
**items** | [**List[ApiV1InvoiceComputePost200ResponseDataItemsInner]**](ApiV1InvoiceComputePost200ResponseDataItemsInner.md) |  | 
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
from intifact_sdk.models.api_v1_invoice_compute_post200_response_data import ApiV1InvoiceComputePost200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceComputePost200ResponseData from a JSON string
api_v1_invoice_compute_post200_response_data_instance = ApiV1InvoiceComputePost200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceComputePost200ResponseData.to_json())

# convert the object into a dict
api_v1_invoice_compute_post200_response_data_dict = api_v1_invoice_compute_post200_response_data_instance.to_dict()
# create an instance of ApiV1InvoiceComputePost200ResponseData from a dict
api_v1_invoice_compute_post200_response_data_from_dict = ApiV1InvoiceComputePost200ResponseData.from_dict(api_v1_invoice_compute_post200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


