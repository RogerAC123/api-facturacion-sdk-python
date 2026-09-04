# ApiV1DocumentsIdRecoverPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**estado** | **str** |  | [optional] 
**codigo** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_documents_id_recover_post200_response import ApiV1DocumentsIdRecoverPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DocumentsIdRecoverPost200Response from a JSON string
api_v1_documents_id_recover_post200_response_instance = ApiV1DocumentsIdRecoverPost200Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1DocumentsIdRecoverPost200Response.to_json())

# convert the object into a dict
api_v1_documents_id_recover_post200_response_dict = api_v1_documents_id_recover_post200_response_instance.to_dict()
# create an instance of ApiV1DocumentsIdRecoverPost200Response from a dict
api_v1_documents_id_recover_post200_response_from_dict = ApiV1DocumentsIdRecoverPost200Response.from_dict(api_v1_documents_id_recover_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


