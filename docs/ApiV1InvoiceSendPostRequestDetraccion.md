# ApiV1InvoiceSendPostRequestDetraccion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cod_bien_servicio** | **str** |  | 
**cuenta_banco** | **str** |  | 
**porcentaje** | **float** |  | 
**monto** | **float** |  | 
**medio_pago** | **str** |  | [optional] [default to '001']

## Example

```python
from intifact_sdk.models.api_v1_invoice_send_post_request_detraccion import ApiV1InvoiceSendPostRequestDetraccion

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1InvoiceSendPostRequestDetraccion from a JSON string
api_v1_invoice_send_post_request_detraccion_instance = ApiV1InvoiceSendPostRequestDetraccion.from_json(json)
# print the JSON string representation of the object
print(ApiV1InvoiceSendPostRequestDetraccion.to_json())

# convert the object into a dict
api_v1_invoice_send_post_request_detraccion_dict = api_v1_invoice_send_post_request_detraccion_instance.to_dict()
# create an instance of ApiV1InvoiceSendPostRequestDetraccion from a dict
api_v1_invoice_send_post_request_detraccion_from_dict = ApiV1InvoiceSendPostRequestDetraccion.from_dict(api_v1_invoice_send_post_request_detraccion_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


