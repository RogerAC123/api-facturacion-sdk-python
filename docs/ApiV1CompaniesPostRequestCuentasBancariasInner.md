# ApiV1CompaniesPostRequestCuentasBancariasInner


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
from intifact_sdk.models.api_v1_companies_post_request_cuentas_bancarias_inner import ApiV1CompaniesPostRequestCuentasBancariasInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CompaniesPostRequestCuentasBancariasInner from a JSON string
api_v1_companies_post_request_cuentas_bancarias_inner_instance = ApiV1CompaniesPostRequestCuentasBancariasInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1CompaniesPostRequestCuentasBancariasInner.to_json())

# convert the object into a dict
api_v1_companies_post_request_cuentas_bancarias_inner_dict = api_v1_companies_post_request_cuentas_bancarias_inner_instance.to_dict()
# create an instance of ApiV1CompaniesPostRequestCuentasBancariasInner from a dict
api_v1_companies_post_request_cuentas_bancarias_inner_from_dict = ApiV1CompaniesPostRequestCuentasBancariasInner.from_dict(api_v1_companies_post_request_cuentas_bancarias_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


