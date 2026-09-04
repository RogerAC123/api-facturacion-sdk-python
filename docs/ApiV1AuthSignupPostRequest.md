# ApiV1AuthSignupPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**password** | **str** |  | 
**name** | **str** |  | [optional] 
**tenant_name** | **str** |  | 

## Example

```python
from intifact_sdk.models.api_v1_auth_signup_post_request import ApiV1AuthSignupPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1AuthSignupPostRequest from a JSON string
api_v1_auth_signup_post_request_instance = ApiV1AuthSignupPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1AuthSignupPostRequest.to_json())

# convert the object into a dict
api_v1_auth_signup_post_request_dict = api_v1_auth_signup_post_request_instance.to_dict()
# create an instance of ApiV1AuthSignupPostRequest from a dict
api_v1_auth_signup_post_request_from_dict = ApiV1AuthSignupPostRequest.from_dict(api_v1_auth_signup_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


