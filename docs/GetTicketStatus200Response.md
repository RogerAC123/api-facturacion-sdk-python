# GetTicketStatus200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**status_code** | **str** |  | 
**cdr_response** | [**GetTicketStatus200ResponseCdrResponse**](GetTicketStatus200ResponseCdrResponse.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.get_ticket_status200_response import GetTicketStatus200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetTicketStatus200Response from a JSON string
get_ticket_status200_response_instance = GetTicketStatus200Response.from_json(json)
# print the JSON string representation of the object
print(GetTicketStatus200Response.to_json())

# convert the object into a dict
get_ticket_status200_response_dict = get_ticket_status200_response_instance.to_dict()
# create an instance of GetTicketStatus200Response from a dict
get_ticket_status200_response_from_dict = GetTicketStatus200Response.from_dict(get_ticket_status200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


