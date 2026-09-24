# intifact_sdk.BranchesApi

All URIs are relative to *http://localhost:3099*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_branches**](BranchesApi.md#list_branches) | **GET** /api/v1/companies/{id}/branches | Listar establecimientos (sucursales) de una empresa


# **list_branches**
> list_branches(id)

Listar establecimientos (sucursales) de una empresa

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:3099
# See configuration.py for a list of all supported configuration parameters.
configuration = intifact_sdk.Configuration(
    host = "http://localhost:3099"
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
    api_instance = intifact_sdk.BranchesApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Listar establecimientos (sucursales) de una empresa
        api_instance.list_branches(id)
    except Exception as e:
        print("Exception when calling BranchesApi->list_branches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

