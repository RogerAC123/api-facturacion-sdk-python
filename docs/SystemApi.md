# intifact_sdk.SystemApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_catalogs_get**](SystemApi.md#api_v1_catalogs_get) | **GET** /api/v1/catalogs | Listar catálogos SUNAT (código → descripción)
[**api_v1_catalogs_key_get**](SystemApi.md#api_v1_catalogs_key_get) | **GET** /api/v1/catalogs/{key} | Obtener un catálogo por clave
[**health_get**](SystemApi.md#health_get) | **GET** /health | Health check del servicio (DB + Redis + SUNAT env)
[**internal_certificates_expiring_get**](SystemApi.md#internal_certificates_expiring_get) | **GET** /internal/certificates/expiring | List certificates expiring within N days (internal)
[**internal_webhooks_stats_get**](SystemApi.md#internal_webhooks_stats_get) | **GET** /internal/webhooks/stats | Webhook delivery statistics (internal)


# **api_v1_catalogs_get**
> ApiV1CatalogsGet200Response api_v1_catalogs_get()

Listar catálogos SUNAT (código → descripción)

Devuelve los catálogos SUNAT más usados y los específicos de guías de remisión (01 tipo doc, 06 doc identidad, 18 modalidad, 20 motivo traslado, 61 doc relacionado, 07 afectación IGV, 25 unidad, etc.).

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_catalogs_get200_response import ApiV1CatalogsGet200Response
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
    api_instance = intifact_sdk.SystemApi(api_client)

    try:
        # Listar catálogos SUNAT (código → descripción)
        api_response = api_instance.api_v1_catalogs_get()
        print("The response of SystemApi->api_v1_catalogs_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->api_v1_catalogs_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiV1CatalogsGet200Response**](ApiV1CatalogsGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_catalogs_key_get**
> api_v1_catalogs_key_get(key)

Obtener un catálogo por clave

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
    api_instance = intifact_sdk.SystemApi(api_client)
    key = 'key_example' # str | 

    try:
        # Obtener un catálogo por clave
        api_instance.api_v1_catalogs_key_get(key)
    except Exception as e:
        print("Exception when calling SystemApi->api_v1_catalogs_key_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 

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

# **health_get**
> health_get()

Health check del servicio (DB + Redis + SUNAT env)

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
    api_instance = intifact_sdk.SystemApi(api_client)

    try:
        # Health check del servicio (DB + Redis + SUNAT env)
        api_instance.health_get()
    except Exception as e:
        print("Exception when calling SystemApi->health_get: %s\n" % e)
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

# **internal_certificates_expiring_get**
> internal_certificates_expiring_get(days=days)

List certificates expiring within N days (internal)

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
    api_instance = intifact_sdk.SystemApi(api_client)
    days = 30 # int |  (optional) (default to 30)

    try:
        # List certificates expiring within N days (internal)
        api_instance.internal_certificates_expiring_get(days=days)
    except Exception as e:
        print("Exception when calling SystemApi->internal_certificates_expiring_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **days** | **int**|  | [optional] [default to 30]

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

# **internal_webhooks_stats_get**
> internal_webhooks_stats_get(days=days)

Webhook delivery statistics (internal)

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
    api_instance = intifact_sdk.SystemApi(api_client)
    days = 7 # int |  (optional) (default to 7)

    try:
        # Webhook delivery statistics (internal)
        api_instance.internal_webhooks_stats_get(days=days)
    except Exception as e:
        print("Exception when calling SystemApi->internal_webhooks_stats_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **days** | **int**|  | [optional] [default to 7]

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

