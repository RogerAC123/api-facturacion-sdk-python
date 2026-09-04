# ApiV1InvoiceCancelPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**motivo_baja** | **str** |  | 
**ra_correlativo** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_invoice_cancel_post_request import ApiV1InvoiceCancelPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceCancelPostRequest from a JSON string
api_v1_invoice_cancel_post_request_instance = ApiV1InvoiceCancelPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceCancelPostRequest.to_json())

# convert the object into a dict
api_v1_invoice_cancel_post_request_dict = api_v1_invoice_cancel_post_request_instance.to_dict()
# create an instance of ApiV1InvoiceCancelPostRequest from a dict
api_v1_invoice_cancel_post_request_from_dict = ApiV1InvoiceCancelPostRequest.from_dict(api_v1_invoice_cancel_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


