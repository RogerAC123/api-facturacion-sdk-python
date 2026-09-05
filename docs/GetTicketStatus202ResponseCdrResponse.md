# GetTicketStatus202ResponseCdrResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**code** | **str** |  | 
**description** | **str** |  | 
**notes** | **List[str]** |  | 

## Example

```python
from intifact_sdk.models.get_ticket_status202_response_cdr_response import GetTicketStatus202ResponseCdrResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GetTicketStatus202ResponseCdrResponse from a JSON string
get_ticket_status202_response_cdr_response_instance = GetTicketStatus202ResponseCdrResponse.from_json(json)
# print the JSON string representation of the object
print(GetTicketStatus202ResponseCdrResponse.to_json())

# convert the object into a dict
get_ticket_status202_response_cdr_response_dict = get_ticket_status202_response_cdr_response_instance.to_dict()
# create an instance of GetTicketStatus202ResponseCdrResponse from a dict
get_ticket_status202_response_cdr_response_from_dict = GetTicketStatus202ResponseCdrResponse.from_dict(get_ticket_status202_response_cdr_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


