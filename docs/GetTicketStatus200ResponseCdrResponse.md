# GetTicketStatus200ResponseCdrResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**code** | **str** |  | 
**description** | **str** |  | 
**notes** | **List[Optional[str]]** |  | 

## Example

```python
from intifact_sdk.models.get_ticket_status200_response_cdr_response import GetTicketStatus200ResponseCdrResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GetTicketStatus200ResponseCdrResponse from a JSON string
get_ticket_status200_response_cdr_response_instance = GetTicketStatus200ResponseCdrResponse.from_json(json)
# print the JSON string representation of the object
print(GetTicketStatus200ResponseCdrResponse.to_json())

# convert the object into a dict
get_ticket_status200_response_cdr_response_dict = get_ticket_status200_response_cdr_response_instance.to_dict()
# create an instance of GetTicketStatus200ResponseCdrResponse from a dict
get_ticket_status200_response_cdr_response_from_dict = GetTicketStatus200ResponseCdrResponse.from_dict(get_ticket_status200_response_cdr_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


