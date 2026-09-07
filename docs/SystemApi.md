# intifact_sdk.SystemApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**export_producto_sunat**](SystemApi.md#export_producto_sunat) | **GET** /api/v1/catalogs/producto/export | Descargar el Catálogo 25 completo (52.840 códigos)
[**get_catalog**](SystemApi.md#get_catalog) | **GET** /api/v1/catalogs/{key} | Obtener un catálogo por clave
[**get_producto_sunat**](SystemApi.md#get_producto_sunat) | **GET** /api/v1/catalogs/producto/{codigo} | Obtener un Código de Producto SUNAT por código
[**health_get**](SystemApi.md#health_get) | **GET** /health | Health check del servicio (DB + Redis + SUNAT env)
[**internal_certificates_expiring_get**](SystemApi.md#internal_certificates_expiring_get) | **GET** /internal/certificates/expiring | List certificates expiring within N days (internal)
[**internal_webhooks_stats_get**](SystemApi.md#internal_webhooks_stats_get) | **GET** /internal/webhooks/stats | Webhook delivery statistics (internal)
[**list_catalogs**](SystemApi.md#list_catalogs) | **GET** /api/v1/catalogs | Listar catálogos SUNAT (código → descripción)
[**search_producto_sunat**](SystemApi.md#search_producto_sunat) | **GET** /api/v1/catalogs/producto/search | Buscar Código de Producto SUNAT (Catálogo 25 / UNSPSC)


# **export_producto_sunat**
> ExportProductoSunat200Response export_producto_sunat()

Descargar el Catálogo 25 completo (52.840 códigos)

Devuelve `{ success, data: { version, total, items[] } }` con TODO el catálogo, en el mismo shape que devuelve la búsqueda. Pensado para cachearlo del lado del integrador: manda `If-None-Match` con el ETag recibido y la API responde 304 si nada cambió. Se sirve con `Content-Encoding: gzip` si el cliente lo acepta (~600 KB vs ~8 MB).

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.export_producto_sunat200_response import ExportProductoSunat200Response
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
    api_instance = intifact_sdk.SystemApi(api_client)

    try:
        # Descargar el Catálogo 25 completo (52.840 códigos)
        api_response = api_instance.export_producto_sunat()
        print("The response of SystemApi->export_producto_sunat:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->export_producto_sunat: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ExportProductoSunat200Response**](ExportProductoSunat200Response.md)

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

# **get_catalog**
> get_catalog(key)

Obtener un catálogo por clave

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
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
    api_instance = intifact_sdk.SystemApi(api_client)
    key = 'key_example' # str | 

    try:
        # Obtener un catálogo por clave
        api_instance.get_catalog(key)
    except Exception as e:
        print("Exception when calling SystemApi->get_catalog: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 

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

# **get_producto_sunat**
> GetProductoSunat200Response get_producto_sunat(codigo)

Obtener un Código de Producto SUNAT por código

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.get_producto_sunat200_response import GetProductoSunat200Response
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
    api_instance = intifact_sdk.SystemApi(api_client)
    codigo = 'codigo_example' # str | 

    try:
        # Obtener un Código de Producto SUNAT por código
        api_response = api_instance.get_producto_sunat(codigo)
        print("The response of SystemApi->get_producto_sunat:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->get_producto_sunat: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **codigo** | **str**|  | 

### Return type

[**GetProductoSunat200Response**](GetProductoSunat200Response.md)

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
**404** | Default Response |  -  |
**429** | Default Response |  -  |

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

* Bearer Authentication (apiKey):

```python
import intifact_sdk
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

# **internal_webhooks_stats_get**
> internal_webhooks_stats_get(days=days)

Webhook delivery statistics (internal)

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
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

# **list_catalogs**
> ListCatalogs200Response list_catalogs()

Listar catálogos SUNAT (código → descripción)

Devuelve los catálogos SUNAT más usados y los específicos de guías de remisión (01 tipo doc, 06 doc identidad, 18 modalidad, 20 motivo traslado, 61 doc relacionado, 07 afectación IGV, 25 unidad, etc.).

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.list_catalogs200_response import ListCatalogs200Response
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
    api_instance = intifact_sdk.SystemApi(api_client)

    try:
        # Listar catálogos SUNAT (código → descripción)
        api_response = api_instance.list_catalogs()
        print("The response of SystemApi->list_catalogs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->list_catalogs: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ListCatalogs200Response**](ListCatalogs200Response.md)

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

# **search_producto_sunat**
> SearchProductoSunat200Response search_producto_sunat(q, nivel=nivel, limit=limit)

Buscar Código de Producto SUNAT (Catálogo 25 / UNSPSC)

Busca por texto libre (sin distinguir tildes ni mayúsculas, todos los términos deben aparecer) o por prefijo de código si `q` son dígitos. Devuelve primero las CLASE: SUNAT exige llegar como mínimo a ese nivel y es la respuesta correcta en la mayoría de casos.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.search_producto_sunat200_response import SearchProductoSunat200Response
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
    api_instance = intifact_sdk.SystemApi(api_client)
    q = 'q_example' # str | 
    nivel = 'nivel_example' # str |  (optional)
    limit = 20 # int |  (optional) (default to 20)

    try:
        # Buscar Código de Producto SUNAT (Catálogo 25 / UNSPSC)
        api_response = api_instance.search_producto_sunat(q, nivel=nivel, limit=limit)
        print("The response of SystemApi->search_producto_sunat:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->search_producto_sunat: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **str**|  | 
 **nivel** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] [default to 20]

### Return type

[**SearchProductoSunat200Response**](SearchProductoSunat200Response.md)

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

