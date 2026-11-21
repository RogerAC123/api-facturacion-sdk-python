# RegisterCompanyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ruc** | **str** |  | 
**razon_social** | **str** |  | 
**nombre_comercial** | **str** |  | [optional] 
**ubigeo** | **str** |  | [optional] 
**direccion** | **str** |  | [optional] 
**departamento** | **str** |  | [optional] 
**provincia** | **str** |  | [optional] 
**distrito** | **str** |  | [optional] 
**urbanizacion** | **str** |  | [optional] 
**telefono** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**web** | **str** |  | [optional] 
**sol_user** | **str** |  | [optional] 
**sol_password** | **str** |  | [optional] 
**certificado** | [**RegisterCompanyRequestCertificado**](RegisterCompanyRequestCertificado.md) |  | 

## Example

```python
from intifact_sdk.models.register_company_request import RegisterCompanyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RegisterCompanyRequest from a JSON string
register_company_request_instance = RegisterCompanyRequest.from_json(json)
# print the JSON string representation of the object
print(RegisterCompanyRequest.to_json())

# convert the object into a dict
register_company_request_dict = register_company_request_instance.to_dict()
# create an instance of RegisterCompanyRequest from a dict
register_company_request_from_dict = RegisterCompanyRequest.from_dict(register_company_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


