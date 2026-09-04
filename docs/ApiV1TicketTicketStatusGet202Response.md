# ApiV1TicketTicketStatusGet202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**status_code** | **str** |  | 
**cdr_response** | [**ApiV1TicketTicketStatusGet202ResponseCdrResponse**](ApiV1TicketTicketStatusGet202ResponseCdrResponse.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.api_v1_ticket_ticket_status_get202_response import ApiV1TicketTicketStatusGet202Response

# TODO update the JSON string below
json = "{}"
# create an instance of ApiV1TicketTicketStatusGet202Response from a JSON string
api_v1_ticket_ticket_status_get202_response_instance = ApiV1TicketTicketStatusGet202Response.from_json(json)
# print the JSON string representation of the object
print(ApiV1TicketTicketStatusGet202Response.to_json())

# convert the object into a dict
api_v1_ticket_ticket_status_get202_response_dict = api_v1_ticket_ticket_status_get202_response_instance.to_dict()
# create an instance of ApiV1TicketTicketStatusGet202Response from a dict
api_v1_ticket_ticket_status_get202_response_from_dict = ApiV1TicketTicketStatusGet202Response.from_dict(api_v1_ticket_ticket_status_get202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


