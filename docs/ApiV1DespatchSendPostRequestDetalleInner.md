# ApiV1DespatchSendPostRequestDetalleInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unidad** | **str** |  | 
**cantidad** | **float** |  | 
**cod_producto** | **str** |  | 
**descripcion** | **str** |  | 

## Example

```python
from intifact_sdk.models.api_v1_despatch_send_post_request_detalle_inner import ApiV1DespatchSendPostRequestDetalleInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchSendPostRequestDetalleInner from a JSON string
api_v1_despatch_send_post_request_detalle_inner_instance = ApiV1DespatchSendPostRequestDetalleInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchSendPostRequestDetalleInner.to_json())

# convert the object into a dict
api_v1_despatch_send_post_request_detalle_inner_dict = api_v1_despatch_send_post_request_detalle_inner_instance.to_dict()
# create an instance of ApiV1DespatchSendPostRequestDetalleInner from a dict
api_v1_despatch_send_post_request_detalle_inner_from_dict = ApiV1DespatchSendPostRequestDetalleInner.from_dict(api_v1_despatch_send_post_request_detalle_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


