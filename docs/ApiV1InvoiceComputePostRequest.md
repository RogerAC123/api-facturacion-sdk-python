# ApiV1InvoiceComputePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_moneda** | **str** |  | [optional] [default to 'PEN']
**items** | [**List[ApiV1InvoiceComputePostRequestItemsInner]**](ApiV1InvoiceComputePostRequestItemsInner.md) |  | 
**descuento_global** | [**ApiV1InvoiceComputePostRequestItemsInnerDescuento**](ApiV1InvoiceComputePostRequestItemsInnerDescuento.md) |  | [optional] 
**precios_incluyen_igv** | **bool** |  | [optional] [default to False]

## Example

```python
from intifact_sdk.models.api_v1_invoice_compute_post_request import ApiV1InvoiceComputePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceComputePostRequest from a JSON string
api_v1_invoice_compute_post_request_instance = ApiV1InvoiceComputePostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceComputePostRequest.to_json())

# convert the object into a dict
api_v1_invoice_compute_post_request_dict = api_v1_invoice_compute_post_request_instance.to_dict()
# create an instance of ApiV1InvoiceComputePostRequest from a dict
api_v1_invoice_compute_post_request_from_dict = ApiV1InvoiceComputePostRequest.from_dict(api_v1_invoice_compute_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


