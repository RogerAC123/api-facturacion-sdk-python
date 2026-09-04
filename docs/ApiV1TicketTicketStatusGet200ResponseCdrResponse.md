# ApiV1TicketTicketStatusGet200ResponseCdrResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**code** | **str** |  | 
**description** | **str** |  | 
**notes** | **List[Optional[str]]** |  | 

## Example

```python
from intifact_sdk.models.api_v1_ticket_ticket_status_get200_response_cdr_response import ApiV1TicketTicketStatusGet200ResponseCdrResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1TicketTicketStatusGet200ResponseCdrResponse from a JSON string
api_v1_ticket_ticket_status_get200_response_cdr_response_instance = ApiV1TicketTicketStatusGet200ResponseCdrResponse.from_json(json)
# print the JSON string representation of the object
print(ApiV1TicketTicketStatusGet200ResponseCdrResponse.to_json())

# convert the object into a dict
api_v1_ticket_ticket_status_get200_response_cdr_response_dict = api_v1_ticket_ticket_status_get200_response_cdr_response_instance.to_dict()
# create an instance of ApiV1TicketTicketStatusGet200ResponseCdrResponse from a dict
api_v1_ticket_ticket_status_get200_response_cdr_response_from_dict = ApiV1TicketTicketStatusGet200ResponseCdrResponse.from_dict(api_v1_ticket_ticket_status_get200_response_cdr_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


