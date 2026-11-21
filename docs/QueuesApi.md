# intifact_sdk.QueuesApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_queue_stats**](QueuesApi.md#get_queue_stats) | **GET** /api/v1/queues/stats | Estado de las colas BullMQ


# **get_queue_stats**
> GetQueueStats200Response get_queue_stats()

Estado de las colas BullMQ

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.get_queue_stats200_response import GetQueueStats200Response
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: apiKey
configuration = intifact_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.QueuesApi(api_client)

    try:
        # Estado de las colas BullMQ
        api_response = api_instance.get_queue_stats()
        print("The response of QueuesApi->get_queue_stats:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueuesApi->get_queue_stats: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**GetQueueStats200Response**](GetQueueStats200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

