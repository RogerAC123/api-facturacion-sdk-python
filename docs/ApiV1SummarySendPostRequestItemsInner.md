# ApiV1SummarySendPostRequestItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**cliente_tipo_doc** | **str** |  | 
**cliente_num_doc** | **str** |  | 
**estado_item** | **str** |  | 
**tipo_moneda** | **str** |  | [optional] [default to 'PEN']
**monto_oper_gravadas** | **float** |  | [optional] [default to 0]
**monto_oper_exoneradas** | **float** |  | [optional] [default to 0]
**monto_oper_inafectas** | **float** |  | [optional] [default to 0]
**monto_oper_gratuitas** | **float** |  | [optional] [default to 0]
**monto_igv** | **float** |  | [optional] [default to 0]
**monto_isc** | **float** |  | [optional] [default to 0]
**monto_otros_cargos** | **float** |  | [optional] [default to 0]
**monto_total** | **float** |  | 

## Example

```python
from intifact_sdk.models.api_v1_summary_send_post_request_items_inner import ApiV1SummarySendPostRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1SummarySendPostRequestItemsInner from a JSON string
api_v1_summary_send_post_request_items_inner_instance = ApiV1SummarySendPostRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1SummarySendPostRequestItemsInner.to_json())

# convert the object into a dict
api_v1_summary_send_post_request_items_inner_dict = api_v1_summary_send_post_request_items_inner_instance.to_dict()
# create an instance of ApiV1SummarySendPostRequestItemsInner from a dict
api_v1_summary_send_post_request_items_inner_from_dict = ApiV1SummarySendPostRequestItemsInner.from_dict(api_v1_summary_send_post_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


