# UpdateCompanyRequestCuentasBancariasInner


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
from intifact_sdk.models.update_company_request_cuentas_bancarias_inner import UpdateCompanyRequestCuentasBancariasInner

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateCompanyRequestCuentasBancariasInner from a JSON string
update_company_request_cuentas_bancarias_inner_instance = UpdateCompanyRequestCuentasBancariasInner.from_json(json)
# print the JSON string representation of the object
print(UpdateCompanyRequestCuentasBancariasInner.to_json())

# convert the object into a dict
update_company_request_cuentas_bancarias_inner_dict = update_company_request_cuentas_bancarias_inner_instance.to_dict()
# create an instance of UpdateCompanyRequestCuentasBancariasInner from a dict
update_company_request_cuentas_bancarias_inner_from_dict = UpdateCompanyRequestCuentasBancariasInner.from_dict(update_company_request_cuentas_bancarias_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


