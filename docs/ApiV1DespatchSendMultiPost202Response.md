# ApiV1DespatchSendMultiPost202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**ApiV1DespatchSendMultiPost202ResponseData**](ApiV1DespatchSendMultiPost202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_despatch_send_multi_post202_response import ApiV1DespatchSendMultiPost202Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1DespatchSendMultiPost202Response from a JSON string
api_v1_despatch_send_multi_post202_response_instance = ApiV1DespatchSendMultiPost202Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1DespatchSendMultiPost202Response.to_json())

# convert the object into a dict
api_v1_despatch_send_multi_post202_response_dict = api_v1_despatch_send_multi_post202_response_instance.to_dict()
# create an instance of ApiV1DespatchSendMultiPost202Response from a dict
api_v1_despatch_send_multi_post202_response_from_dict = ApiV1DespatchSendMultiPost202Response.from_dict(api_v1_despatch_send_multi_post202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


