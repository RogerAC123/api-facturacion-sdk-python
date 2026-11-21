# CreateBranchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**codigo** | **str** |  | 
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
from intifact_sdk.models.create_branch_request import CreateBranchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateBranchRequest from a JSON string
create_branch_request_instance = CreateBranchRequest.from_json(json)
# print the JSON string representation of the object
print(CreateBranchRequest.to_json())

# convert the object into a dict
create_branch_request_dict = create_branch_request_instance.to_dict()
# create an instance of CreateBranchRequest from a dict
create_branch_request_from_dict = CreateBranchRequest.from_dict(create_branch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


