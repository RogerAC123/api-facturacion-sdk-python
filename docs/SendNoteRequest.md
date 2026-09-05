# SendNoteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo_operacion** | **str** |  | [optional] [default to '0101']
**tipo_doc** | **str** |  | 
**serie** | **str** |  | 
**correlativo** | **str** |  | 
**tipo_moneda** | **str** |  | [optional] [default to 'PEN']
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
**afectado_tipo_doc** | **str** |  | 
**afectado_num_doc** | **str** |  | 
**motivo_cod** | **str** |  | 
**motivo_des** | **str** |  | 
**monto_oper_gravadas** | **float** |  | [optional] [default to 0]
**monto_oper_exoneradas** | **float** |  | [optional] [default to 0]
**monto_oper_inafectas** | **float** |  | [optional] [default to 0]
**monto_igv** | **float** |  | 
**total_impuestos** | **float** |  | 
**valor_venta** | **float** |  | 
**sub_total** | **float** |  | 
**monto_imp_venta** | **float** |  | 
**descuento_global** | **float** |  | [optional] 
**descuento_global_base** | **float** |  | [optional] 
**detalle** | [**List[SendInvoiceRequestDetalleInner]**](SendInvoiceRequestDetalleInner.md) |  | 
**leyendas** | [**List[SendInvoiceRequestLeyendasInner]**](SendInvoiceRequestLeyendasInner.md) |  | 
**observacion** | **str** |  | [optional] 

## Example

```python
from intifact_sdk.models.send_note_request import SendNoteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendNoteRequest from a JSON string
send_note_request_instance = SendNoteRequest.from_json(json)
# print the JSON string representation of the object
print(SendNoteRequest.to_json())

# convert the object into a dict
send_note_request_dict = send_note_request_instance.to_dict()
# create an instance of SendNoteRequest from a dict
send_note_request_from_dict = SendNoteRequest.from_dict(send_note_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


