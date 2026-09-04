# ApiV1CompaniesPostRequest


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
**tenant_id** | **UUID** |  | [optional] 
**gre_client_id** | **str** |  | [optional] 
**gre_client_secret** | **str** |  | [optional] 
**sunat_production** | **bool** |  | [optional] 
**cuentas_bancarias** | [**List[ApiV1CompaniesPostRequestCuentasBancariasInner]**](ApiV1CompaniesPostRequestCuentasBancariasInner.md) |  | [optional] 
**terminos_titulo** | **str** |  | [optional] 
**terminos** | **List[str]** |  | [optional] 
**nota_pago_titulo** | **str** |  | [optional] 
**nota_pago_texto** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_companies_post_request import ApiV1CompaniesPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CompaniesPostRequest from a JSON string
api_v1_companies_post_request_instance = ApiV1CompaniesPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1CompaniesPostRequest.to_json())

# convert the object into a dict
api_v1_companies_post_request_dict = api_v1_companies_post_request_instance.to_dict()
# create an instance of ApiV1CompaniesPostRequest from a dict
api_v1_companies_post_request_from_dict = ApiV1CompaniesPostRequest.from_dict(api_v1_companies_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


