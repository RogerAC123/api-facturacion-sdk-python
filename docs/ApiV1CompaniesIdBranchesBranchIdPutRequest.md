# ApiV1CompaniesIdBranchesBranchIdPutRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**nombre** | **str** |  | [optional] 
**ubigeo** | **str** |  | [optional] 
**direccion** | **str** |  | [optional] 
**departamento** | **str** |  | [optional] 
**provincia** | **str** |  | [optional] 
**distrito** | **str** |  | [optional] 
**urbanizacion** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] [default to True]

## Example

```python
from intifact_sdk.models.api_v1_companies_id_branches_branch_id_put_request import ApiV1CompaniesIdBranchesBranchIdPutRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CompaniesIdBranchesBranchIdPutRequest from a JSON string
api_v1_companies_id_branches_branch_id_put_request_instance = ApiV1CompaniesIdBranchesBranchIdPutRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1CompaniesIdBranchesBranchIdPutRequest.to_json())

# convert the object into a dict
api_v1_companies_id_branches_branch_id_put_request_dict = api_v1_companies_id_branches_branch_id_put_request_instance.to_dict()
# create an instance of ApiV1CompaniesIdBranchesBranchIdPutRequest from a dict
api_v1_companies_id_branches_branch_id_put_request_from_dict = ApiV1CompaniesIdBranchesBranchIdPutRequest.from_dict(api_v1_companies_id_branches_branch_id_put_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


