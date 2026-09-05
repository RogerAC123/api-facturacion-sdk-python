# SendDespatchRequestDocumentosRelacionadosInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cod_tipo** | **str** |  | 
**numero** | **str** |  | 
**tipo_desc** | **str** |  | [optional] 
**emisor_ruc** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.send_despatch_request_documentos_relacionados_inner import SendDespatchRequestDocumentosRelacionadosInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchRequestDocumentosRelacionadosInner from a JSON string
send_despatch_request_documentos_relacionados_inner_instance = SendDespatchRequestDocumentosRelacionadosInner.from_json(json)
# print the JSON string representation of the object
print(SendDespatchRequestDocumentosRelacionadosInner.to_json())

# convert the object into a dict
send_despatch_request_documentos_relacionados_inner_dict = send_despatch_request_documentos_relacionados_inner_instance.to_dict()
# create an instance of SendDespatchRequestDocumentosRelacionadosInner from a dict
send_despatch_request_documentos_relacionados_inner_from_dict = SendDespatchRequestDocumentosRelacionadosInner.from_dict(send_despatch_request_documentos_relacionados_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


