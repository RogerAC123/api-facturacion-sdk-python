# ApiV1NoteComputePostRequestItemsInner


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
**descuento** | [**ApiV1InvoiceComputePostRequestItemsInnerDescuento**](ApiV1InvoiceComputePostRequestItemsInnerDescuento.md) |  | [optional] 
**factor_icbper** | **float** |  | [optional] [default to 0]
**marca** | **str** |  | [optional] 
**cod_prod_sunat** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_note_compute_post_request_items_inner import ApiV1NoteComputePostRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1NoteComputePostRequestItemsInner from a JSON string
api_v1_note_compute_post_request_items_inner_instance = ApiV1NoteComputePostRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1NoteComputePostRequestItemsInner.to_json())

# convert the object into a dict
api_v1_note_compute_post_request_items_inner_dict = api_v1_note_compute_post_request_items_inner_instance.to_dict()
# create an instance of ApiV1NoteComputePostRequestItemsInner from a dict
api_v1_note_compute_post_request_items_inner_from_dict = ApiV1NoteComputePostRequestItemsInner.from_dict(api_v1_note_compute_post_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


