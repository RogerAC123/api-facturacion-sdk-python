# ComputeInvoice200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**ComputeInvoice200ResponseData**](ComputeInvoice200ResponseData.md) |  | 

## Example

```python
from intifact_sdk.models.compute_invoice200_response import ComputeInvoice200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ComputeInvoice200Response from a JSON string
compute_invoice200_response_instance = ComputeInvoice200Response.from_json(json)
# print the JSON string representation of the object
print(ComputeInvoice200Response.to_json())

# convert the object into a dict
compute_invoice200_response_dict = compute_invoice200_response_instance.to_dict()
# create an instance of ComputeInvoice200Response from a dict
compute_invoice200_response_from_dict = ComputeInvoice200Response.from_dict(compute_invoice200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


