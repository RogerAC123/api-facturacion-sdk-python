# SendSummaryRequestItemsInner


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
from intifact_sdk.models.send_summary_request_items_inner import SendSummaryRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendSummaryRequestItemsInner from a JSON string
send_summary_request_items_inner_instance = SendSummaryRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(SendSummaryRequestItemsInner.to_json())

# convert the object into a dict
send_summary_request_items_inner_dict = send_summary_request_items_inner_instance.to_dict()
# create an instance of SendSummaryRequestItemsInner from a dict
send_summary_request_items_inner_from_dict = SendSummaryRequestItemsInner.from_dict(send_summary_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


