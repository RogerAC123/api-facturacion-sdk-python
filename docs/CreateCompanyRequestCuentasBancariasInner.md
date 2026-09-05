# CreateCompanyRequestCuentasBancariasInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**nombre** | **str** |  | 
**bancos** | **List[str]** |  | [optional] [default to []]
**tipo_label** | **str** |  | 
**titular_label** | **str** |  | [optional] 
**titular** | **str** |  | [optional] 
**titular_ruc** | **str** |  | [optional] 
**numero** | **str** |  | 
**cci** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.create_company_request_cuentas_bancarias_inner import CreateCompanyRequestCuentasBancariasInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCompanyRequestCuentasBancariasInner from a JSON string
create_company_request_cuentas_bancarias_inner_instance = CreateCompanyRequestCuentasBancariasInner.from_json(json)
# print the JSON string representation of the object
print(CreateCompanyRequestCuentasBancariasInner.to_json())

# convert the object into a dict
create_company_request_cuentas_bancarias_inner_dict = create_company_request_cuentas_bancarias_inner_instance.to_dict()
# create an instance of CreateCompanyRequestCuentasBancariasInner from a dict
create_company_request_cuentas_bancarias_inner_from_dict = CreateCompanyRequestCuentasBancariasInner.from_dict(create_company_request_cuentas_bancarias_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


