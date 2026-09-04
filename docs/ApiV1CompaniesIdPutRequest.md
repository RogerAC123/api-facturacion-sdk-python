# ApiV1CompaniesIdPutRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ruc** | **str** |  | [optional] 
**razon_social** | **str** |  | [optional] 
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
from intifact_sdk.models.api_v1_companies_id_put_request import ApiV1CompaniesIdPutRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1CompaniesIdPutRequest from a JSON string
api_v1_companies_id_put_request_instance = ApiV1CompaniesIdPutRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1CompaniesIdPutRequest.to_json())

# convert the object into a dict
api_v1_companies_id_put_request_dict = api_v1_companies_id_put_request_instance.to_dict()
# create an instance of ApiV1CompaniesIdPutRequest from a dict
api_v1_companies_id_put_request_from_dict = ApiV1CompaniesIdPutRequest.from_dict(api_v1_companies_id_put_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


