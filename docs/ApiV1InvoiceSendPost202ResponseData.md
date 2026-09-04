# ApiV1InvoiceSendPost202ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**estado** | **str** |  | 
**hash** | **str** |  | 
**signature_value** | **str** |  | 
**job_id** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post202_response_data import ApiV1InvoiceSendPost202ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPost202ResponseData from a JSON string
api_v1_invoice_send_post202_response_data_instance = ApiV1InvoiceSendPost202ResponseData.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPost202ResponseData.to_json())

# convert the object into a dict
api_v1_invoice_send_post202_response_data_dict = api_v1_invoice_send_post202_response_data_instance.to_dict()
# create an instance of ApiV1InvoiceSendPost202ResponseData from a dict
api_v1_invoice_send_post202_response_data_from_dict = ApiV1InvoiceSendPost202ResponseData.from_dict(api_v1_invoice_send_post202_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


