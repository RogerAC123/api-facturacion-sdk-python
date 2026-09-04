# ApiV1InvoiceComputePost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**ApiV1InvoiceComputePost200ResponseData**](ApiV1InvoiceComputePost200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_invoice_compute_post200_response import ApiV1InvoiceComputePost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceComputePost200Response from a JSON string
api_v1_invoice_compute_post200_response_instance = ApiV1InvoiceComputePost200Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceComputePost200Response.to_json())

# convert the object into a dict
api_v1_invoice_compute_post200_response_dict = api_v1_invoice_compute_post200_response_instance.to_dict()
# create an instance of ApiV1InvoiceComputePost200Response from a dict
api_v1_invoice_compute_post200_response_from_dict = ApiV1InvoiceComputePost200Response.from_dict(api_v1_invoice_compute_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


