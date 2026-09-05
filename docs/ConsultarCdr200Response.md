# ConsultarCdr200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**available** | **bool** |  | 
**message** | **str** |  | 
**status_code** | **str** |  | [optional] 
**codigo** | **str** |  | [optional] 
**descripcion** | **str** |  | [optional] 
**cdr_zip_base64** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.consultar_cdr200_response import ConsultarCdr200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ConsultarCdr200Response from a JSON string
consultar_cdr200_response_instance = ConsultarCdr200Response.from_json(json)
# print the JSON string representation of the object
print(ConsultarCdr200Response.to_json())

# convert the object into a dict
consultar_cdr200_response_dict = consultar_cdr200_response_instance.to_dict()
# create an instance of ConsultarCdr200Response from a dict
consultar_cdr200_response_from_dict = ConsultarCdr200Response.from_dict(consultar_cdr200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


