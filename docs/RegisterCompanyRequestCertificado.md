# RegisterCompanyRequestCertificado


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** | Base64 del .p12/.pfx | 
**password** | **str** |  | 
**name** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.register_company_request_certificado import RegisterCompanyRequestCertificado

# TODO update the JSON string below
json = "{}"
# create an instance of RegisterCompanyRequestCertificado from a JSON string
register_company_request_certificado_instance = RegisterCompanyRequestCertificado.from_json(json)
# print the JSON string representation of the object
print(RegisterCompanyRequestCertificado.to_json())

# convert the object into a dict
register_company_request_certificado_dict = register_company_request_certificado_instance.to_dict()
# create an instance of RegisterCompanyRequestCertificado from a dict
register_company_request_certificado_from_dict = RegisterCompanyRequestCertificado.from_dict(register_company_request_certificado_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


