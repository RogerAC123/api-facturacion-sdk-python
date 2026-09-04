# ApiV1AuthLoginPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from intifact_sdk.models.api_v1_auth_login_post_request import ApiV1AuthLoginPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1AuthLoginPostRequest from a JSON string
api_v1_auth_login_post_request_instance = ApiV1AuthLoginPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1AuthLoginPostRequest.to_json())

# convert the object into a dict
api_v1_auth_login_post_request_dict = api_v1_auth_login_post_request_instance.to_dict()
# create an instance of ApiV1AuthLoginPostRequest from a dict
api_v1_auth_login_post_request_from_dict = ApiV1AuthLoginPostRequest.from_dict(api_v1_auth_login_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


