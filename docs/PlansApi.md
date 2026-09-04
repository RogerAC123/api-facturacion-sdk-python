# intifact_sdk.PlansApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_plans_get**](PlansApi.md#api_v1_plans_get) | **GET** /api/v1/plans | Listar planes (solo master)
[**api_v1_plans_id_delete**](PlansApi.md#api_v1_plans_id_delete) | **DELETE** /api/v1/plans/{id} | Desactivar plan (soft-delete)
[**api_v1_plans_id_put**](PlansApi.md#api_v1_plans_id_put) | **PUT** /api/v1/plans/{id} | Actualizar plan (precio, docs, nombre, estado)
[**api_v1_plans_post**](PlansApi.md#api_v1_plans_post) | **POST** /api/v1/plans | Crear plan


# **api_v1_plans_get**
> api_v1_plans_get()

Listar planes (solo master)

### Example


```python
import intifact_sdk
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
    api_instance = intifact_sdk.PlansApi(api_client)

    try:
        # Listar planes (solo master)
        api_instance.api_v1_plans_get()
    except Exception as e:
        print("Exception when calling PlansApi->api_v1_plans_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_plans_id_delete**
> api_v1_plans_id_delete(id)

Desactivar plan (soft-delete)

### Example


```python
import intifact_sdk
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
    api_instance = intifact_sdk.PlansApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Desactivar plan (soft-delete)
        api_instance.api_v1_plans_id_delete(id)
    except Exception as e:
        print("Exception when calling PlansApi->api_v1_plans_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_plans_id_put**
> api_v1_plans_id_put(id, api_v1_plans_id_put_request)

Actualizar plan (precio, docs, nombre, estado)

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_plans_id_put_request import ApiV1PlansIdPutRequest
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
    api_instance = intifact_sdk.PlansApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    api_v1_plans_id_put_request = intifact_sdk.ApiV1PlansIdPutRequest() # ApiV1PlansIdPutRequest | 

    try:
        # Actualizar plan (precio, docs, nombre, estado)
        api_instance.api_v1_plans_id_put(id, api_v1_plans_id_put_request)
    except Exception as e:
        print("Exception when calling PlansApi->api_v1_plans_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **api_v1_plans_id_put_request** | [**ApiV1PlansIdPutRequest**](ApiV1PlansIdPutRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_plans_post**
> api_v1_plans_post(api_v1_plans_post_request)

Crear plan

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_plans_post_request import ApiV1PlansPostRequest
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
    api_instance = intifact_sdk.PlansApi(api_client)
    api_v1_plans_post_request = intifact_sdk.ApiV1PlansPostRequest() # ApiV1PlansPostRequest | 

    try:
        # Crear plan
        api_instance.api_v1_plans_post(api_v1_plans_post_request)
    except Exception as e:
        print("Exception when calling PlansApi->api_v1_plans_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_plans_post_request** | [**ApiV1PlansPostRequest**](ApiV1PlansPostRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

