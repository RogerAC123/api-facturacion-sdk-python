# intifact_sdk.WebhooksApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_webhooks_get**](WebhooksApi.md#api_v1_webhooks_get) | **GET** /api/v1/webhooks | Listar webhooks (filtra por RUC opcional)
[**api_v1_webhooks_id_delete**](WebhooksApi.md#api_v1_webhooks_id_delete) | **DELETE** /api/v1/webhooks/{id} | Eliminar webhook (también elimina su historial de deliveries)
[**api_v1_webhooks_id_deliveries_delivery_id_redeliver_post**](WebhooksApi.md#api_v1_webhooks_id_deliveries_delivery_id_redeliver_post) | **POST** /api/v1/webhooks/{id}/deliveries/{deliveryId}/redeliver | Reintentar manualmente una entrega
[**api_v1_webhooks_id_deliveries_get**](WebhooksApi.md#api_v1_webhooks_id_deliveries_get) | **GET** /api/v1/webhooks/{id}/deliveries | Log de entregas del webhook
[**api_v1_webhooks_id_get**](WebhooksApi.md#api_v1_webhooks_id_get) | **GET** /api/v1/webhooks/{id} | Detalle de webhook (sin secret)
[**api_v1_webhooks_id_put**](WebhooksApi.md#api_v1_webhooks_id_put) | **PUT** /api/v1/webhooks/{id} | Actualizar webhook (url, eventos, activación)
[**api_v1_webhooks_id_rotate_secret_post**](WebhooksApi.md#api_v1_webhooks_id_rotate_secret_post) | **POST** /api/v1/webhooks/{id}/rotate-secret | Rotar el secret de firma (devuelto UNA sola vez)
[**api_v1_webhooks_id_test_post**](WebhooksApi.md#api_v1_webhooks_id_test_post) | **POST** /api/v1/webhooks/{id}/test | Enviar un evento de prueba (webhook.test)
[**api_v1_webhooks_post**](WebhooksApi.md#api_v1_webhooks_post) | **POST** /api/v1/webhooks | Crear endpoint webhook


# **api_v1_webhooks_get**
> api_v1_webhooks_get(ruc=ruc)

Listar webhooks (filtra por RUC opcional)

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    ruc = 'ruc_example' # str |  (optional)

    try:
        # Listar webhooks (filtra por RUC opcional)
        api_instance.api_v1_webhooks_get(ruc=ruc)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | [optional] 

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

# **api_v1_webhooks_id_delete**
> api_v1_webhooks_id_delete(id)

Eliminar webhook (también elimina su historial de deliveries)

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Eliminar webhook (también elimina su historial de deliveries)
        api_instance.api_v1_webhooks_id_delete(id)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_delete: %s\n" % e)
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

# **api_v1_webhooks_id_deliveries_delivery_id_redeliver_post**
> api_v1_webhooks_id_deliveries_delivery_id_redeliver_post(id, delivery_id)

Reintentar manualmente una entrega

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    delivery_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Reintentar manualmente una entrega
        api_instance.api_v1_webhooks_id_deliveries_delivery_id_redeliver_post(id, delivery_id)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_deliveries_delivery_id_redeliver_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **delivery_id** | **UUID**|  | 

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

# **api_v1_webhooks_id_deliveries_get**
> api_v1_webhooks_id_deliveries_get(id, limit=limit, success=success)

Log de entregas del webhook

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    limit = 50 # int |  (optional) (default to 50)
    success = 'success_example' # str |  (optional)

    try:
        # Log de entregas del webhook
        api_instance.api_v1_webhooks_id_deliveries_get(id, limit=limit, success=success)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_deliveries_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **limit** | **int**|  | [optional] [default to 50]
 **success** | **str**|  | [optional] 

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

# **api_v1_webhooks_id_get**
> api_v1_webhooks_id_get(id)

Detalle de webhook (sin secret)

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Detalle de webhook (sin secret)
        api_instance.api_v1_webhooks_id_get(id)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_get: %s\n" % e)
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

# **api_v1_webhooks_id_put**
> api_v1_webhooks_id_put(id, api_v1_webhooks_id_put_request)

Actualizar webhook (url, eventos, activación)

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_webhooks_id_put_request import ApiV1WebhooksIdPutRequest
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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    api_v1_webhooks_id_put_request = intifact_sdk.ApiV1WebhooksIdPutRequest() # ApiV1WebhooksIdPutRequest | 

    try:
        # Actualizar webhook (url, eventos, activación)
        api_instance.api_v1_webhooks_id_put(id, api_v1_webhooks_id_put_request)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **api_v1_webhooks_id_put_request** | [**ApiV1WebhooksIdPutRequest**](ApiV1WebhooksIdPutRequest.md)|  | 

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

# **api_v1_webhooks_id_rotate_secret_post**
> api_v1_webhooks_id_rotate_secret_post(id)

Rotar el secret de firma (devuelto UNA sola vez)

Genera un nuevo secret HMAC y lo devuelve una única vez. Las firmas de entregas posteriores usarán el nuevo secret; actualiza tu receptor antes de rotar.

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Rotar el secret de firma (devuelto UNA sola vez)
        api_instance.api_v1_webhooks_id_rotate_secret_post(id)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_rotate_secret_post: %s\n" % e)
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

# **api_v1_webhooks_id_test_post**
> api_v1_webhooks_id_test_post(id)

Enviar un evento de prueba (webhook.test)

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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Enviar un evento de prueba (webhook.test)
        api_instance.api_v1_webhooks_id_test_post(id)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_id_test_post: %s\n" % e)
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

# **api_v1_webhooks_post**
> api_v1_webhooks_post(api_v1_webhooks_post_request)

Crear endpoint webhook

Registra una URL que recibirá POSTs cuando ocurran los eventos suscritos. Sin `empresaRuc` el webhook cubre TODAS las empresas de tu cuenta (un solo secret; el `empresaRuc` viaja en cada payload). La respuesta incluye el `secret` (mostrado UNA sola vez) — guárdalo para verificar las firmas HMAC-SHA256.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_webhooks_post_request import ApiV1WebhooksPostRequest
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
    api_instance = intifact_sdk.WebhooksApi(api_client)
    api_v1_webhooks_post_request = intifact_sdk.ApiV1WebhooksPostRequest() # ApiV1WebhooksPostRequest | 

    try:
        # Crear endpoint webhook
        api_instance.api_v1_webhooks_post(api_v1_webhooks_post_request)
    except Exception as e:
        print("Exception when calling WebhooksApi->api_v1_webhooks_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_webhooks_post_request** | [**ApiV1WebhooksPostRequest**](ApiV1WebhooksPostRequest.md)|  | 

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

