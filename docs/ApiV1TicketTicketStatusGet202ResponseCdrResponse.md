# ApiV1TicketTicketStatusGet202ResponseCdrResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**code** | **str** |  | 
**description** | **str** |  | 
**notes** | **List[str]** |  | 

## Example

```python
from intifact_sdk.models.api_v1_ticket_ticket_status_get202_response_cdr_response import ApiV1TicketTicketStatusGet202ResponseCdrResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1TicketTicketStatusGet202ResponseCdrResponse from a JSON string
api_v1_ticket_ticket_status_get202_response_cdr_response_instance = ApiV1TicketTicketStatusGet202ResponseCdrResponse.from_json(json)
# print the JSON string representation of the object
print(ApiV1TicketTicketStatusGet202ResponseCdrResponse.to_json())

# convert the object into a dict
api_v1_ticket_ticket_status_get202_response_cdr_response_dict = api_v1_ticket_ticket_status_get202_response_cdr_response_instance.to_dict()
# create an instance of ApiV1TicketTicketStatusGet202ResponseCdrResponse from a dict
api_v1_ticket_ticket_status_get202_response_cdr_response_from_dict = ApiV1TicketTicketStatusGet202ResponseCdrResponse.from_dict(api_v1_ticket_ticket_status_get202_response_cdr_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


