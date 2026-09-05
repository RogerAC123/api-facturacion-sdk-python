# intifact_sdk.DocumentsApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**consultar_cdr**](DocumentsApi.md#consultar_cdr) | **POST** /api/v1/cdr/consultar | Consultar el CDR de un comprobante en SUNAT por referencia
[**get_document**](DocumentsApi.md#get_document) | **GET** /api/v1/documents/{id} | Detalle completo de un documento
[**get_next_correlativo**](DocumentsApi.md#get_next_correlativo) | **GET** /api/v1/documents/next-correlativo | Obtener el siguiente correlativo disponible para una serie
[**list_documents**](DocumentsApi.md#list_documents) | **GET** /api/v1/documents | Listar documentos con filtros y paginación
[**reconcile_document**](DocumentsApi.md#reconcile_document) | **POST** /api/v1/documents/{id}/recover | Reconciliar un documento con SUNAT (consulta de CDR, solo master)
[**retry_document**](DocumentsApi.md#retry_document) | **POST** /api/v1/documents/{id}/retry | Re-encolar un documento fallido


# **consultar_cdr**
> ConsultarCdr200Response consultar_cdr(consultar_cdr_request)

Consultar el CDR de un comprobante en SUNAT por referencia

Recupera el CDR oficial (billConsultService / getStatusCdr) de un comprobante 01/03/07/08 por RUC+serie+número, aunque no exista en esta BD. Útil para recuperar el histórico emitido por otro PSE. Solo en producción; usa la Clave SOL de la empresa (debe existir y estar en scope de la API key).

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.consultar_cdr200_response import ConsultarCdr200Response
from intifact_sdk.models.consultar_cdr_request import ConsultarCdrRequest
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    consultar_cdr_request = intifact_sdk.ConsultarCdrRequest() # ConsultarCdrRequest | 

    try:
        # Consultar el CDR de un comprobante en SUNAT por referencia
        api_response = api_instance.consultar_cdr(consultar_cdr_request)
        print("The response of DocumentsApi->consultar_cdr:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->consultar_cdr: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **consultar_cdr_request** | [**ConsultarCdrRequest**](ConsultarCdrRequest.md)|  | 

### Return type

[**ConsultarCdr200Response**](ConsultarCdr200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_document**
> get_document(id)

Detalle completo de un documento

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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Detalle completo de un documento
        api_instance.get_document(id)
    except Exception as e:
        print("Exception when calling DocumentsApi->get_document: %s\n" % e)
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

# **get_next_correlativo**
> GetNextCorrelativo200Response get_next_correlativo(company_ruc, tipo_doc, serie)

Obtener el siguiente correlativo disponible para una serie

Busca el correlativo más alto existente para la combinación empresa+tipoDoc+serie y retorna el siguiente. Útil para auto-numeración.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.get_next_correlativo200_response import GetNextCorrelativo200Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    company_ruc = 'company_ruc_example' # str | 
    tipo_doc = 'tipo_doc_example' # str | 
    serie = 'serie_example' # str | 

    try:
        # Obtener el siguiente correlativo disponible para una serie
        api_response = api_instance.get_next_correlativo(company_ruc, tipo_doc, serie)
        print("The response of DocumentsApi->get_next_correlativo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->get_next_correlativo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **company_ruc** | **str**|  | 
 **tipo_doc** | **str**|  | 
 **serie** | **str**|  | 

### Return type

[**GetNextCorrelativo200Response**](GetNextCorrelativo200Response.md)

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

# **list_documents**
> ListDocuments200Response list_documents(ruc=ruc, tipo_doc=tipo_doc, serie=serie, estado=estado, env=env, fecha_desde=fecha_desde, fecha_hasta=fecha_hasta, cliente_num_doc=cliente_num_doc, page=page, limit=limit)

Listar documentos con filtros y paginación

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.list_documents200_response import ListDocuments200Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    ruc = 'ruc_example' # str |  (optional)
    tipo_doc = 'tipo_doc_example' # str |  (optional)
    serie = 'serie_example' # str |  (optional)
    estado = 'estado_example' # str |  (optional)
    env = 'env_example' # str |  (optional)
    fecha_desde = 'fecha_desde_example' # str |  (optional)
    fecha_hasta = 'fecha_hasta_example' # str |  (optional)
    cliente_num_doc = 'cliente_num_doc_example' # str |  (optional)
    page = 1 # int |  (optional) (default to 1)
    limit = 20 # int |  (optional) (default to 20)

    try:
        # Listar documentos con filtros y paginación
        api_response = api_instance.list_documents(ruc=ruc, tipo_doc=tipo_doc, serie=serie, estado=estado, env=env, fecha_desde=fecha_desde, fecha_hasta=fecha_hasta, cliente_num_doc=cliente_num_doc, page=page, limit=limit)
        print("The response of DocumentsApi->list_documents:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->list_documents: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | [optional] 
 **tipo_doc** | **str**|  | [optional] 
 **serie** | **str**|  | [optional] 
 **estado** | **str**|  | [optional] 
 **env** | **str**|  | [optional] 
 **fecha_desde** | **str**|  | [optional] 
 **fecha_hasta** | **str**|  | [optional] 
 **cliente_num_doc** | **str**|  | [optional] 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 20]

### Return type

[**ListDocuments200Response**](ListDocuments200Response.md)

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

# **reconcile_document**
> ReconcileDocument200Response reconcile_document(id)

Reconciliar un documento con SUNAT (consulta de CDR, solo master)

Consulta el estado REAL en SUNAT (getStatusCdr / billConsultService) SIN reenviar y corrige la BD. Útil cuando un documento quedó desincronizado (ej. una boleta ACEPTADA figurando RECHAZADO/COLA_FALLIDA/ENCOLADO). Solo comprobantes 01/03/07/08, solo en producción. Restringido al master API key.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.reconcile_document200_response import ReconcileDocument200Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Reconciliar un documento con SUNAT (consulta de CDR, solo master)
        api_response = api_instance.reconcile_document(id)
        print("The response of DocumentsApi->reconcile_document:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->reconcile_document: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

[**ReconcileDocument200Response**](ReconcileDocument200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **retry_document**
> RetryDocument202Response retry_document(id)

Re-encolar un documento fallido

Útil cuando un documento quedó en estado COLA_FALLIDA tras agotar los reintentos automáticos.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.retry_document202_response import RetryDocument202Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Re-encolar un documento fallido
        api_response = api_instance.retry_document(id)
        print("The response of DocumentsApi->retry_document:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->retry_document: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

[**RetryDocument202Response**](RetryDocument202Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

