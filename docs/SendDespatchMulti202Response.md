# SendDespatchMulti202Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  | 
**message** | **str** |  | 
**data** | [**SendDespatchMulti202ResponseData**](SendDespatchMulti202ResponseData.md) |  | [optional] 

## Example

```python
from intifact_sdk.models.send_despatch_multi202_response import SendDespatchMulti202Response

# TODO update the JSON string below
json = "{}"
# create an instance of SendDespatchMulti202Response from a JSON string
send_despatch_multi202_response_instance = SendDespatchMulti202Response.from_json(json)
# print the JSON string representation of the object
print(SendDespatchMulti202Response.to_json())

# convert the object into a dict
send_despatch_multi202_response_dict = send_despatch_multi202_response_instance.to_dict()
# create an instance of SendDespatchMulti202Response from a dict
send_despatch_multi202_response_from_dict = SendDespatchMulti202Response.from_dict(send_despatch_multi202_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


