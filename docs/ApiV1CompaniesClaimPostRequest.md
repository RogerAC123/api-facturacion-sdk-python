# ApiV1CompaniesClaimPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ruc** | **str** |  | 
**password** | **str** |  | 
**content** | **str** | Base64 del .p12/.pfx | 
**name** | **str** |  | [optional] 
**razon_social** | **str** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_companies_claim_post_request import ApiV1CompaniesClaimPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CompaniesClaimPostRequest from a JSON string
api_v1_companies_claim_post_request_instance = ApiV1CompaniesClaimPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1CompaniesClaimPostRequest.to_json())

# convert the object into a dict
api_v1_companies_claim_post_request_dict = api_v1_companies_claim_post_request_instance.to_dict()
# create an instance of ApiV1CompaniesClaimPostRequest from a dict
api_v1_companies_claim_post_request_from_dict = ApiV1CompaniesClaimPostRequest.from_dict(api_v1_companies_claim_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


