# UpdateBranchRequest


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
from intifact_sdk.models.update_branch_request import UpdateBranchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateBranchRequest from a JSON string
update_branch_request_instance = UpdateBranchRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateBranchRequest.to_json())

# convert the object into a dict
update_branch_request_dict = update_branch_request_instance.to_dict()
# create an instance of UpdateBranchRequest from a dict
update_branch_request_from_dict = UpdateBranchRequest.from_dict(update_branch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


