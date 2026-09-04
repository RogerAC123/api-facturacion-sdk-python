# ApiV1NoteSendPostRequestDetalleInner


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
from intifact_sdk.models.api_v1_note_send_post_request_detalle_inner import ApiV1NoteSendPostRequestDetalleInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1NoteSendPostRequestDetalleInner from a JSON string
api_v1_note_send_post_request_detalle_inner_instance = ApiV1NoteSendPostRequestDetalleInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1NoteSendPostRequestDetalleInner.to_json())

# convert the object into a dict
api_v1_note_send_post_request_detalle_inner_dict = api_v1_note_send_post_request_detalle_inner_instance.to_dict()
# create an instance of ApiV1NoteSendPostRequestDetalleInner from a dict
api_v1_note_send_post_request_detalle_inner_from_dict = ApiV1NoteSendPostRequestDetalleInner.from_dict(api_v1_note_send_post_request_detalle_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


