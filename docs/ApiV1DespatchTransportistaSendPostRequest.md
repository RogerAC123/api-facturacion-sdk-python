# ApiV1DespatchTransportistaSendPostRequest


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
**chofer** | [**List[ApiV1DespatchSendPostRequestChoferInner]**](ApiV1DespatchSendPostRequestChoferInner.md) |  | 
**guia_vehiculo_placa** | **str** |  | 
**guia_vehiculo_tuc** | **str** |  | [optional] 
**vehiculos_secundarios** | [**List[ApiV1DespatchTransportistaSendPostRequestVehiculosSecundariosInner]**](ApiV1DespatchTransportistaSendPostRequestVehiculosSecundariosInner.md) |  | [optional] 
**guia_partida_ubigeo** | **str** |  | 
**guia_partida_direccion** | **str** |  | 
**guia_llegada_ubigeo** | **str** |  | 
**guia_llegada_direccion** | **str** |  | 
**documentos_relacionados** | [**List[ApiV1DespatchSendPostRequestDocumentosRelacionadosInner]**](ApiV1DespatchSendPostRequestDocumentosRelacionadosInner.md) |  | [optional] 
**detalle** | [**List[ApiV1DespatchSendPostRequestDetalleInner]**](ApiV1DespatchSendPostRequestDetalleInner.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_despatch_transportista_send_post_request import ApiV1DespatchTransportistaSendPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchTransportistaSendPostRequest from a JSON string
api_v1_despatch_transportista_send_post_request_instance = ApiV1DespatchTransportistaSendPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchTransportistaSendPostRequest.to_json())

# convert the object into a dict
api_v1_despatch_transportista_send_post_request_dict = api_v1_despatch_transportista_send_post_request_instance.to_dict()
# create an instance of ApiV1DespatchTransportistaSendPostRequest from a dict
api_v1_despatch_transportista_send_post_request_from_dict = ApiV1DespatchTransportistaSendPostRequest.from_dict(api_v1_despatch_transportista_send_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


