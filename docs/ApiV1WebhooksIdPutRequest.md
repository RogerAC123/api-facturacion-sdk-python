# ApiV1WebhooksIdPutRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**events** | **List[str]** |  | [optional] 
**description** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_webhooks_id_put_request import ApiV1WebhooksIdPutRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1WebhooksIdPutRequest from a JSON string
api_v1_webhooks_id_put_request_instance = ApiV1WebhooksIdPutRequest.from_json(json)
# print the JSON string representation of the object
print(ApiV1WebhooksIdPutRequest.to_json())

# convert the object into a dict
api_v1_webhooks_id_put_request_dict = api_v1_webhooks_id_put_request_instance.to_dict()
# create an instance of ApiV1WebhooksIdPutRequest from a dict
api_v1_webhooks_id_put_request_from_dict = ApiV1WebhooksIdPutRequest.from_dict(api_v1_webhooks_id_put_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


