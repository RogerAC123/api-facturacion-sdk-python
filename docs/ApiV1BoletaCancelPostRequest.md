# ApiV1BoletaCancelPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**empresa_ruc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**motivo_baja** | **str** |  | 
**rc_correlativo** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_boleta_cancel_post_request import ApiV1BoletaCancelPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1BoletaCancelPostRequest from a JSON string
api_v1_boleta_cancel_post_request_instance = ApiV1BoletaCancelPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1BoletaCancelPostRequest.to_json())

# convert the object into a dict
api_v1_boleta_cancel_post_request_dict = api_v1_boleta_cancel_post_request_instance.to_dict()
# create an instance of ApiV1BoletaCancelPostRequest from a dict
api_v1_boleta_cancel_post_request_from_dict = ApiV1BoletaCancelPostRequest.from_dict(api_v1_boleta_cancel_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


