# ApiV1CdrConsultarPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**available** | **bool** |  | 
**message** | **str** |  | 
**status_code** | **str** |  | [optional] 
**codigo** | **str** |  | [optional] 
**descripcion** | **str** |  | [optional] 
**cdr_zip_base64** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_cdr_consultar_post200_response import ApiV1CdrConsultarPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CdrConsultarPost200Response from a JSON string
api_v1_cdr_consultar_post200_response_instance = ApiV1CdrConsultarPost200Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1CdrConsultarPost200Response.to_json())

# convert the object into a dict
api_v1_cdr_consultar_post200_response_dict = api_v1_cdr_consultar_post200_response_instance.to_dict()
# create an instance of ApiV1CdrConsultarPost200Response from a dict
api_v1_cdr_consultar_post200_response_from_dict = ApiV1CdrConsultarPost200Response.from_dict(api_v1_cdr_consultar_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


