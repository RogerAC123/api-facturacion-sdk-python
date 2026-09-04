# ApiV1DespatchSendMultiPost202ResponseDataGuiasInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**code** | **str** |  | [optional] 
**destino** | **float** |  | 
**data** | [**ApiV1NoteSendPost202ResponseData**](ApiV1NoteSendPost202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_despatch_send_multi_post202_response_data_guias_inner import ApiV1DespatchSendMultiPost202ResponseDataGuiasInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchSendMultiPost202ResponseDataGuiasInner from a JSON string
api_v1_despatch_send_multi_post202_response_data_guias_inner_instance = ApiV1DespatchSendMultiPost202ResponseDataGuiasInner.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchSendMultiPost202ResponseDataGuiasInner.to_json())

# convert the object into a dict
api_v1_despatch_send_multi_post202_response_data_guias_inner_dict = api_v1_despatch_send_multi_post202_response_data_guias_inner_instance.to_dict()
# create an instance of ApiV1DespatchSendMultiPost202ResponseDataGuiasInner from a dict
api_v1_despatch_send_multi_post202_response_data_guias_inner_from_dict = ApiV1DespatchSendMultiPost202ResponseDataGuiasInner.from_dict(api_v1_despatch_send_multi_post202_response_data_guias_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


