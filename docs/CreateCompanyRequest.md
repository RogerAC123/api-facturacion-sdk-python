# CreateCompanyRequest


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
**cuentas_bancarias** | [**List[CreateCompanyRequestCuentasBancariasInner]**](CreateCompanyRequestCuentasBancariasInner.md) |  | [optional] 
**terminos_titulo** | **str** |  | [optional] 
**terminos** | **List[str]** |  | [optional] 
**nota_pago_titulo** | **str** |  | [optional] 
**nota_pago_texto** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.create_company_request import CreateCompanyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCompanyRequest from a JSON string
create_company_request_instance = CreateCompanyRequest.from_json(json)
# print the JSON string representation of the object
print(CreateCompanyRequest.to_json())

# convert the object into a dict
create_company_request_dict = create_company_request_instance.to_dict()
# create an instance of CreateCompanyRequest from a dict
create_company_request_from_dict = CreateCompanyRequest.from_dict(create_company_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


