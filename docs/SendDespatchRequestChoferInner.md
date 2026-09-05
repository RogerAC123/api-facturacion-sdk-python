# SendDespatchRequestChoferInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tipo** | **str** |  | 
**tipo_doc** | **str** |  | 
**nro_doc** | **str** |  | 
**licencia** | **str** |  | 
**nombres** | **str** |  | 
**apellidos** | **str** |  | 

## Example

```python
from intifact_sdk.models.send_despatch_request_chofer_inner import SendDespatchRequestChoferInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchRequestChoferInner from a JSON string
send_despatch_request_chofer_inner_instance = SendDespatchRequestChoferInner.from_json(json)
# print the JSON string representation of the object
print(SendDespatchRequestChoferInner.to_json())

# convert the object into a dict
send_despatch_request_chofer_inner_dict = send_despatch_request_chofer_inner_instance.to_dict()
# create an instance of SendDespatchRequestChoferInner from a dict
send_despatch_request_chofer_inner_from_dict = SendDespatchRequestChoferInner.from_dict(send_despatch_request_chofer_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


