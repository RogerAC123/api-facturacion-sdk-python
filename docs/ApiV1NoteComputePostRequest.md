# ApiV1NoteComputePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_moneda** | **str** |  | [optional] [default to 'PEN']
**items** | [**List[ApiV1NoteComputePostRequestItemsInner]**](ApiV1NoteComputePostRequestItemsInner.md) |  | 
**descuento_global** | [**ApiV1InvoiceComputePostRequestItemsInnerDescuento**](ApiV1InvoiceComputePostRequestItemsInnerDescuento.md) |  | [optional] 
**precios_incluyen_igv** | **bool** |  | [optional] [default to False]

## Example

```python
from intifact_sdk.models.api_v1_note_compute_post_request import ApiV1NoteComputePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1NoteComputePostRequest from a JSON string
api_v1_note_compute_post_request_instance = ApiV1NoteComputePostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1NoteComputePostRequest.to_json())

# convert the object into a dict
api_v1_note_compute_post_request_dict = api_v1_note_compute_post_request_instance.to_dict()
# create an instance of ApiV1NoteComputePostRequest from a dict
api_v1_note_compute_post_request_from_dict = ApiV1NoteComputePostRequest.from_dict(api_v1_note_compute_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


