# SendDespatchTransportistaRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**observacion** | **str** |  | [optional] 
**fecha_emision** | **str** |  | 
**empresa_ruc** | **str** |  | 
**establecimiento_codigo** | **str** |  | [optional] [default to '0000']
**transportista_nro_mtc** | **str** |  | [optional] 
**destinatario_tipo_doc** | **str** |  | 
**destinatario_num_doc** | **str** |  | 
**destinatario_razon_social** | **str** |  | 
**destinatario_direccion** | **str** |  | [optional] 
**destinatario_distrito** | **str** |  | [optional] 
**destinatario_provincia** | **str** |  | [optional] 
**destinatario_departamento** | **str** |  | [optional] 
**destinatario_contacto** | **str** |  | [optional] 
**destinatario_telefono** | **str** |  | [optional] 
**destinatario_email** | **str** |  | [optional] 
**entrega_referencia** | **str** |  | [optional] 
**modalidad_entrega** | **str** |  | [optional] 
**agencia_nombre** | **str** |  | [optional] 
**agencia_sede** | **str** |  | [optional] 
**remitente_tipo_doc** | **str** |  | 
**remitente_num_doc** | **str** |  | 
**remitente_razon_social** | **str** |  | 
**guia_cod_traslado** | **str** |  | 
**guia_des_traslado** | **str** |  | [optional] 
**guia_peso_total** | **float** |  | 
**guia_und_peso_total** | **str** |  | [optional] [default to 'KGM']
**guia_num_bultos** | **int** |  | [optional] 
**guia_fec_traslado** | **str** |  | 
**chofer** | [**List[SendDespatchRequestChoferInner]**](SendDespatchRequestChoferInner.md) |  | 
**guia_vehiculo_placa** | **str** |  | 
**guia_vehiculo_tuc** | **str** |  | [optional] 
**vehiculos_secundarios** | [**List[SendDespatchTransportistaRequestVehiculosSecundariosInner]**](SendDespatchTransportistaRequestVehiculosSecundariosInner.md) |  | [optional] 
**guia_partida_ubigeo** | **str** |  | 
**guia_partida_direccion** | **str** |  | 
**guia_llegada_ubigeo** | **str** |  | 
**guia_llegada_direccion** | **str** |  | 
**documentos_relacionados** | [**List[SendDespatchRequestDocumentosRelacionadosInner]**](SendDespatchRequestDocumentosRelacionadosInner.md) |  | [optional] 
**detalle** | [**List[SendDespatchRequestDetalleInner]**](SendDespatchRequestDetalleInner.md) |  | 

## Example

```python
from intifact_sdk.models.send_despatch_transportista_request import SendDespatchTransportistaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchTransportistaRequest from a JSON string
send_despatch_transportista_request_instance = SendDespatchTransportistaRequest.from_json(json)
# print the JSON string representation of the object
print(SendDespatchTransportistaRequest.to_json())

# convert the object into a dict
send_despatch_transportista_request_dict = send_despatch_transportista_request_instance.to_dict()
# create an instance of SendDespatchTransportistaRequest from a dict
send_despatch_transportista_request_from_dict = SendDespatchTransportistaRequest.from_dict(send_despatch_transportista_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


