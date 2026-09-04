# ApiV1DespatchSendMultiPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**observacion** | **str** |  | [optional] 
**fecha_emision** | **str** |  | 
**empresa_ruc** | **str** |  | 
**establecimiento_codigo** | **str** |  | [optional] [default to '0000']
**guia_cod_traslado** | **str** |  | 
**guia_mod_traslado** | **str** |  | 
**guia_fec_traslado** | **str** |  | 
**guia_vehiculo_placa** | **str** |  | [optional] 
**transportista_tipo_doc** | **str** |  | [optional] 
**transportista_num_doc** | **str** |  | [optional] 
**transportista_razon_social** | **str** |  | [optional] 
**transportista_nro_mtc** | **str** |  | [optional] 
**guia_partida_ubigeo** | **str** |  | 
**guia_partida_direccion** | **str** |  | 
**chofer** | [**List[ApiV1DespatchSendPostRequestChoferInner]**](ApiV1DespatchSendPostRequestChoferInner.md) |  | [optional] 
**guia_fec_entrega** | **str** |  | [optional] 
**guia_des_traslado** | **str** |  | [optional] 
**guia_peso_neto** | **float** |  | [optional] 
**guia_sustento_peso** | **str** |  | [optional] 
**guia_num_bultos** | **int** |  | [optional] 
**indicadores** | [**ApiV1DespatchSendPostRequestIndicadores**](ApiV1DespatchSendPostRequestIndicadores.md) |  | [optional] 
**contenedores** | [**List[ApiV1DespatchSendPostRequestContenedoresInner]**](ApiV1DespatchSendPostRequestContenedoresInner.md) |  | [optional] 
**guia_vehiculo_tuc** | **str** |  | [optional] 
**guia_vehiculo_autorizacion** | **str** |  | [optional] 
**guia_vehiculo_autorizacion_entidad** | **str** |  | [optional] 
**vehiculos_secundarios** | [**List[ApiV1DespatchSendPostRequestVehiculosSecundariosInner]**](ApiV1DespatchSendPostRequestVehiculosSecundariosInner.md) |  | [optional] 
**transportista_autorizacion** | **str** |  | [optional] 
**transportista_autorizacion_entidad** | **str** |  | [optional] 
**guia_partida_ruc** | **str** |  | [optional] 
**guia_partida_cod_local** | **str** |  | [optional] 
**guia_partida_geo** | [**ApiV1DespatchSendPostRequestGuiaLlegadaGeo**](ApiV1DespatchSendPostRequestGuiaLlegadaGeo.md) |  | [optional] 
**guia_llegada_ruc** | **str** |  | [optional] 
**guia_llegada_cod_local** | **str** |  | [optional] 
**guia_llegada_geo** | [**ApiV1DespatchSendPostRequestGuiaLlegadaGeo**](ApiV1DespatchSendPostRequestGuiaLlegadaGeo.md) |  | [optional] 
**documentos_relacionados** | [**List[ApiV1DespatchSendPostRequestDocumentosRelacionadosInner]**](ApiV1DespatchSendPostRequestDocumentosRelacionadosInner.md) |  | [optional] 
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
**destinos** | [**List[ApiV1DespatchSendMultiPostRequestDestinosInner]**](ApiV1DespatchSendMultiPostRequestDestinosInner.md) |  | 

## Example

```python
from intifact_sdk.models.api_v1_despatch_send_multi_post_request import ApiV1DespatchSendMultiPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchSendMultiPostRequest from a JSON string
api_v1_despatch_send_multi_post_request_instance = ApiV1DespatchSendMultiPostRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchSendMultiPostRequest.to_json())

# convert the object into a dict
api_v1_despatch_send_multi_post_request_dict = api_v1_despatch_send_multi_post_request_instance.to_dict()
# create an instance of ApiV1DespatchSendMultiPostRequest from a dict
api_v1_despatch_send_multi_post_request_from_dict = ApiV1DespatchSendMultiPostRequest.from_dict(api_v1_despatch_send_multi_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


