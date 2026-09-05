# SendInvoiceRequestDetalleInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unidad** | **str** |  | 
**cantidad** | **float** |  | 
**cod_producto** | **str** |  | 
**descripcion** | **str** |  | 
**marca** | **str** |  | [optional] 
**monto_valor_unitario** | **float** |  | 
**monto_base_igv** | **float** |  | 
**porcentaje_igv** | **float** |  | [optional] [default to 18]
**igv** | **float** |  | 
**tip_afe_igv** | **str** |  | [optional] [default to '10']
**total_impuestos** | **float** |  | 
**monto_precio_unitario** | **float** |  | 
**monto_valor_venta** | **float** |  | 
**descuento** | **float** |  | [optional] 
**descuento_item** | **float** |  | [optional] 
**factor_icbper** | **float** |  | [optional] [default to 0]
**cod_prod_sunat** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.send_invoice_request_detalle_inner import SendInvoiceRequestDetalleInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequestDetalleInner from a JSON string
send_invoice_request_detalle_inner_instance = SendInvoiceRequestDetalleInner.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequestDetalleInner.to_json())

# convert the object into a dict
send_invoice_request_detalle_inner_dict = send_invoice_request_detalle_inner_instance.to_dict()
# create an instance of SendInvoiceRequestDetalleInner from a dict
send_invoice_request_detalle_inner_from_dict = SendInvoiceRequestDetalleInner.from_dict(send_invoice_request_detalle_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


