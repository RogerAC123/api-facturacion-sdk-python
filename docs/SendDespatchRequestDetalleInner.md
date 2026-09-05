# SendDespatchRequestDetalleInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unidad** | **str** |  | 
**cantidad** | **float** |  | 
**cod_producto** | **str** |  | 
**descripcion** | **str** |  | 

## Example

```python
from intifact_sdk.models.send_despatch_request_detalle_inner import SendDespatchRequestDetalleInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchRequestDetalleInner from a JSON string
send_despatch_request_detalle_inner_instance = SendDespatchRequestDetalleInner.from_json(json)
# print the JSON string representation of the object
print(SendDespatchRequestDetalleInner.to_json())

# convert the object into a dict
send_despatch_request_detalle_inner_dict = send_despatch_request_detalle_inner_instance.to_dict()
# create an instance of SendDespatchRequestDetalleInner from a dict
send_despatch_request_detalle_inner_from_dict = SendDespatchRequestDetalleInner.from_dict(send_despatch_request_detalle_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


