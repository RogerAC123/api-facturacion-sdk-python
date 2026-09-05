# InternalCertificatesExpiringGet401Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**code** | **str** |  | [optional] 
**errors** | [**List[InternalCertificatesExpiringGet401ResponseErrorsInner]**](InternalCertificatesExpiringGet401ResponseErrorsInner.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.internal_certificates_expiring_get401_response import InternalCertificatesExpiringGet401Response

# TODO update the JSON string below
json = "{}"
# create an instance of InternalCertificatesExpiringGet401Response from a JSON string
internal_certificates_expiring_get401_response_instance = InternalCertificatesExpiringGet401Response.from_json(json)
# print the JSON string representation of the object
print(InternalCertificatesExpiringGet401Response.to_json())

# convert the object into a dict
internal_certificates_expiring_get401_response_dict = internal_certificates_expiring_get401_response_instance.to_dict()
# create an instance of InternalCertificatesExpiringGet401Response from a dict
internal_certificates_expiring_get401_response_from_dict = InternalCertificatesExpiringGet401Response.from_dict(internal_certificates_expiring_get401_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


