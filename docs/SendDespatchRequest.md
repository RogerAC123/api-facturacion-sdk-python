# SendDespatchRequest


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
**cliente_tipo_doc** | **str** |  | 
**cliente_num_doc** | **str** |  | 
**cliente_razon_social** | **str** |  | 
**cliente_direccion** | **str** |  | [optional] 
**cliente_distrito** | **str** |  | [optional] 
**cliente_provincia** | **str** |  | [optional] 
**cliente_departamento** | **str** |  | [optional] 
**destinatario_contacto** | **str** |  | [optional] 
**destinatario_telefono** | **str** |  | [optional] 
**destinatario_email** | **str** |  | [optional] 
**entrega_referencia** | **str** |  | [optional] 
**modalidad_entrega** | **str** |  | [optional] 
**agencia_nombre** | **str** |  | [optional] 
**agencia_sede** | **str** |  | [optional] 
**guia_cod_traslado** | **str** |  | 
**guia_mod_traslado** | **str** |  | 
**guia_peso_total** | **float** |  | 
**guia_und_peso_total** | **str** |  | [optional] [default to 'KGM']
**guia_fec_traslado** | **str** |  | 
**guia_vehiculo_placa** | **str** |  | [optional] 
**transportista_tipo_doc** | **str** |  | [optional] 
**transportista_num_doc** | **str** |  | [optional] 
**transportista_razon_social** | **str** |  | [optional] 
**transportista_nro_mtc** | **str** |  | [optional] 
**guia_partida_ubigeo** | **str** |  | 
**guia_partida_direccion** | **str** |  | 
**guia_partida_ciudad** | **str** |  | [optional] 
**guia_llegada_ubigeo** | **str** |  | 
**guia_llegada_direccion** | **str** |  | 
**guia_llegada_ciudad** | **str** |  | [optional] 
**chofer** | [**List[SendDespatchRequestChoferInner]**](SendDespatchRequestChoferInner.md) |  | [optional] 
**guia_fec_entrega** | **str** |  | [optional] 
**guia_des_traslado** | **str** |  | [optional] 
**guia_peso_neto** | **float** |  | [optional] 
**guia_sustento_peso** | **str** |  | [optional] 
**guia_num_bultos** | **int** |  | [optional] 
**indicadores** | [**SendDespatchRequestIndicadores**](SendDespatchRequestIndicadores.md) |  | [optional] 
**contenedores** | [**List[SendDespatchRequestContenedoresInner]**](SendDespatchRequestContenedoresInner.md) |  | [optional] 
**guia_vehiculo_tuc** | **str** |  | [optional] 
**guia_vehiculo_autorizacion** | **str** |  | [optional] 
**guia_vehiculo_autorizacion_entidad** | **str** |  | [optional] 
**vehiculos_secundarios** | [**List[SendDespatchRequestVehiculosSecundariosInner]**](SendDespatchRequestVehiculosSecundariosInner.md) |  | [optional] 
**transportista_autorizacion** | **str** |  | [optional] 
**transportista_autorizacion_entidad** | **str** |  | [optional] 
**guia_partida_ruc** | **str** |  | [optional] 
**guia_partida_cod_local** | **str** |  | [optional] 
**guia_partida_geo** | [**SendDespatchRequestGuiaPartidaGeo**](SendDespatchRequestGuiaPartidaGeo.md) |  | [optional] 
**guia_llegada_ruc** | **str** |  | [optional] 
**guia_llegada_cod_local** | **str** |  | [optional] 
**guia_llegada_geo** | [**SendDespatchRequestGuiaLlegadaGeo**](SendDespatchRequestGuiaLlegadaGeo.md) |  | [optional] 
**documentos_relacionados** | [**List[SendDespatchRequestDocumentosRelacionadosInner]**](SendDespatchRequestDocumentosRelacionadosInner.md) |  | [optional] 
**remitente_autorizacion** | **str** |  | [optional] 
**remitente_autorizacion_entidad** | **str** |  | [optional] 
**proveedor_tipo_doc** | **str** |  | [optional] 
**proveedor_num_doc** | **str** |  | [optional] 
**proveedor_razon_social** | **str** |  | [optional] 
**comprador_tipo_doc** | **str** |  | [optional] 
**comprador_num_doc** | **str** |  | [optional] 
**comprador_razon_social** | **str** |  | [optional] 
**puerto_codigo** | **str** |  | [optional] 
**puerto_nombre** | **str** |  | [optional] 
**puerto_tipo** | **str** |  | [optional] 
**detalle** | [**List[SendDespatchRequestDetalleInner]**](SendDespatchRequestDetalleInner.md) |  | 

## Example

```python
from intifact_sdk.models.send_despatch_request import SendDespatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchRequest from a JSON string
send_despatch_request_instance = SendDespatchRequest.from_json(json)
# print the JSON string representation of the object
print(SendDespatchRequest.to_json())

# convert the object into a dict
send_despatch_request_dict = send_despatch_request_instance.to_dict()
# create an instance of SendDespatchRequest from a dict
send_despatch_request_from_dict = SendDespatchRequest.from_dict(send_despatch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


