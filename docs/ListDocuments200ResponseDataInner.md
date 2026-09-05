# ListDocuments200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**env** | **str** |  | 
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**fecha_emision** | **str** |  | 
**tipo_moneda** | **str** |  | 
**cliente_num_doc** | **str** |  | 
**cliente_razon_social** | **str** |  | 
**monto_imp_venta** | **str** |  | 
**monto_igv** | **str** |  | [optional] 
**estado_sunat** | **str** |  | 
**codigo_respuesta** | **str** |  | 
**descripcion_respuesta** | **str** |  | [optional] 
**hash_cdr** | **str** |  | 
**created_at** | **str** |  | 
**company** | [**ListDocuments200ResponseDataInnerCompany**](ListDocuments200ResponseDataInnerCompany.md) |  | 

## Example

```python
from intifact_sdk.models.list_documents200_response_data_inner import ListDocuments200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListDocuments200ResponseDataInner from a JSON string
list_documents200_response_data_inner_instance = ListDocuments200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListDocuments200ResponseDataInner.to_json())

# convert the object into a dict
list_documents200_response_data_inner_dict = list_documents200_response_data_inner_instance.to_dict()
# create an instance of ListDocuments200ResponseDataInner from a dict
list_documents200_response_data_inner_from_dict = ListDocuments200ResponseDataInner.from_dict(list_documents200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


