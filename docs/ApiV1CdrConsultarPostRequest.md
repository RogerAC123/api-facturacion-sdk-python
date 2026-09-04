# ApiV1CdrConsultarPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ruc** | **str** |  | 
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**numero** | **str** |  | 

## Example

```python
from intifact_sdk.models.api_v1_cdr_consultar_post_request import ApiV1CdrConsultarPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CdrConsultarPostRequest from a JSON string
api_v1_cdr_consultar_post_request_instance = ApiV1CdrConsultarPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1CdrConsultarPostRequest.to_json())

# convert the object into a dict
api_v1_cdr_consultar_post_request_dict = api_v1_cdr_consultar_post_request_instance.to_dict()
# create an instance of ApiV1CdrConsultarPostRequest from a dict
api_v1_cdr_consultar_post_request_from_dict = ApiV1CdrConsultarPostRequest.from_dict(api_v1_cdr_consultar_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


