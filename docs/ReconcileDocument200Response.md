# ReconcileDocument200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**estado** | **str** |  | [optional] 
**codigo** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.reconcile_document200_response import ReconcileDocument200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ReconcileDocument200Response from a JSON string
reconcile_document200_response_instance = ReconcileDocument200Response.from_json(json)
# print the JSON string representation of the object
print(ReconcileDocument200Response.to_json())

# convert the object into a dict
reconcile_document200_response_dict = reconcile_document200_response_instance.to_dict()
# create an instance of ReconcileDocument200Response from a dict
reconcile_document200_response_from_dict = ReconcileDocument200Response.from_dict(reconcile_document200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


