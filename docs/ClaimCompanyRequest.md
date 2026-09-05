# ClaimCompanyRequest


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
from intifact_sdk.models.claim_company_request import ClaimCompanyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ClaimCompanyRequest from a JSON string
claim_company_request_instance = ClaimCompanyRequest.from_json(json)
# print the JSON string representation of the object
print(ClaimCompanyRequest.to_json())

# convert the object into a dict
claim_company_request_dict = claim_company_request_instance.to_dict()
# create an instance of ClaimCompanyRequest from a dict
claim_company_request_from_dict = ClaimCompanyRequest.from_dict(claim_company_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


