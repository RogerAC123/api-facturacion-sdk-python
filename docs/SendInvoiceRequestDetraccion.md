# SendInvoiceRequestDetraccion


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
from intifact_sdk.models.send_invoice_request_detraccion import SendInvoiceRequestDetraccion

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceRequestDetraccion from a JSON string
send_invoice_request_detraccion_instance = SendInvoiceRequestDetraccion.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceRequestDetraccion.to_json())

# convert the object into a dict
send_invoice_request_detraccion_dict = send_invoice_request_detraccion_instance.to_dict()
# create an instance of SendInvoiceRequestDetraccion from a dict
send_invoice_request_detraccion_from_dict = SendInvoiceRequestDetraccion.from_dict(send_invoice_request_detraccion_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


