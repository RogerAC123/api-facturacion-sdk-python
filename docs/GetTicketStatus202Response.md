# GetTicketStatus202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**status_code** | **str** |  | 
**cdr_response** | [**GetTicketStatus202ResponseCdrResponse**](GetTicketStatus202ResponseCdrResponse.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.get_ticket_status202_response import GetTicketStatus202Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetTicketStatus202Response from a JSON string
get_ticket_status202_response_instance = GetTicketStatus202Response.from_json(json)
# print the JSON string representation of the object
print(GetTicketStatus202Response.to_json())

# convert the object into a dict
get_ticket_status202_response_dict = get_ticket_status202_response_instance.to_dict()
# create an instance of GetTicketStatus202Response from a dict
get_ticket_status202_response_from_dict = GetTicketStatus202Response.from_dict(get_ticket_status202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


