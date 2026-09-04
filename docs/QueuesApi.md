# intifact_sdk.QueuesApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_queues_stats_get**](QueuesApi.md#api_v1_queues_stats_get) | **GET** /api/v1/queues/stats | Estado de las colas BullMQ


# **api_v1_queues_stats_get**
> ApiV1QueuesStatsGet200Response api_v1_queues_stats_get()

Estado de las colas BullMQ

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_queues_stats_get200_response import ApiV1QueuesStatsGet200Response
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3000
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3000"
)


# Enter a context with an instance of the API client
with intifact_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = intifact_sdk.QueuesApi(api_client)

    try:
        # Estado de las colas BullMQ
        api_response = api_instance.api_v1_queues_stats_get()
        print("The response of QueuesApi->api_v1_queues_stats_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueuesApi->api_v1_queues_stats_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiV1QueuesStatsGet200Response**](ApiV1QueuesStatsGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

