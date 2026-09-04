# intifact_sdk.DocumentsApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_cdr_consultar_post**](DocumentsApi.md#api_v1_cdr_consultar_post) | **POST** /api/v1/cdr/consultar | Consultar el CDR de un comprobante en SUNAT por referencia
[**api_v1_documents_get**](DocumentsApi.md#api_v1_documents_get) | **GET** /api/v1/documents | Listar documentos con filtros y paginación
[**api_v1_documents_id_get**](DocumentsApi.md#api_v1_documents_id_get) | **GET** /api/v1/documents/{id} | Detalle completo de un documento
[**api_v1_documents_id_recover_post**](DocumentsApi.md#api_v1_documents_id_recover_post) | **POST** /api/v1/documents/{id}/recover | Reconciliar un documento con SUNAT (consulta de CDR, solo master)
[**api_v1_documents_id_retry_post**](DocumentsApi.md#api_v1_documents_id_retry_post) | **POST** /api/v1/documents/{id}/retry | Re-encolar un documento fallido
[**api_v1_documents_next_correlativo_get**](DocumentsApi.md#api_v1_documents_next_correlativo_get) | **GET** /api/v1/documents/next-correlativo | Obtener el siguiente correlativo disponible para una serie


# **api_v1_cdr_consultar_post**
> ApiV1CdrConsultarPost200Response api_v1_cdr_consultar_post(api_v1_cdr_consultar_post_request)

Consultar el CDR de un comprobante en SUNAT por referencia

Recupera el CDR oficial (billConsultService / getStatusCdr) de un comprobante 01/03/07/08 por RUC+serie+número, aunque no exista en esta BD. Útil para recuperar el histórico emitido por otro PSE. Solo en producción; usa la Clave SOL de la empresa (debe existir y estar en scope de la API key).

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_cdr_consultar_post200_response import ApiV1CdrConsultarPost200Response
from intifact_sdk.models.api_v1_cdr_consultar_post_request import ApiV1CdrConsultarPostRequest
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    api_v1_cdr_consultar_post_request = intifact_sdk.ApiV1CdrConsultarPostRequest() # ApiV1CdrConsultarPostRequest | 

    try:
        # Consultar el CDR de un comprobante en SUNAT por referencia
        api_response = api_instance.api_v1_cdr_consultar_post(api_v1_cdr_consultar_post_request)
        print("The response of DocumentsApi->api_v1_cdr_consultar_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->api_v1_cdr_consultar_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_cdr_consultar_post_request** | [**ApiV1CdrConsultarPostRequest**](ApiV1CdrConsultarPostRequest.md)|  | 

### Return type

[**ApiV1CdrConsultarPost200Response**](ApiV1CdrConsultarPost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_documents_get**
> ApiV1DocumentsGet200Response api_v1_documents_get(ruc=ruc, tipo_doc=tipo_doc, serie=serie, estado=estado, env=env, fecha_desde=fecha_desde, fecha_hasta=fecha_hasta, cliente_num_doc=cliente_num_doc, page=page, limit=limit)

Listar documentos con filtros y paginación

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_documents_get200_response import ApiV1DocumentsGet200Response
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
        api_response = api_instance.api_v1_documents_get(ruc=ruc, tipo_doc=tipo_doc, serie=serie, estado=estado, env=env, fecha_desde=fecha_desde, fecha_hasta=fecha_hasta, cliente_num_doc=cliente_num_doc, page=page, limit=limit)
        print("The response of DocumentsApi->api_v1_documents_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->api_v1_documents_get: %s\n" % e)
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

[**ApiV1DocumentsGet200Response**](ApiV1DocumentsGet200Response.md)

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

# **api_v1_documents_id_get**
> api_v1_documents_id_get(id)

Detalle completo de un documento

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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Detalle completo de un documento
        api_instance.api_v1_documents_id_get(id)
    except Exception as e:
        print("Exception when calling DocumentsApi->api_v1_documents_id_get: %s\n" % e)
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

# **api_v1_documents_id_recover_post**
> ApiV1DocumentsIdRecoverPost200Response api_v1_documents_id_recover_post(id)

Reconciliar un documento con SUNAT (consulta de CDR, solo master)

Consulta el estado REAL en SUNAT (getStatusCdr / billConsultService) SIN reenviar y corrige la BD. Útil cuando un documento quedó desincronizado (ej. una boleta ACEPTADA figurando RECHAZADO/COLA_FALLIDA/ENCOLADO). Solo comprobantes 01/03/07/08, solo en producción. Restringido al master API key.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_documents_id_recover_post200_response import ApiV1DocumentsIdRecoverPost200Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Reconciliar un documento con SUNAT (consulta de CDR, solo master)
        api_response = api_instance.api_v1_documents_id_recover_post(id)
        print("The response of DocumentsApi->api_v1_documents_id_recover_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->api_v1_documents_id_recover_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

[**ApiV1DocumentsIdRecoverPost200Response**](ApiV1DocumentsIdRecoverPost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_documents_id_retry_post**
> ApiV1DocumentsIdRetryPost202Response api_v1_documents_id_retry_post(id)

Re-encolar un documento fallido

Útil cuando un documento quedó en estado COLA_FALLIDA tras agotar los reintentos automáticos.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_documents_id_retry_post202_response import ApiV1DocumentsIdRetryPost202Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Re-encolar un documento fallido
        api_response = api_instance.api_v1_documents_id_retry_post(id)
        print("The response of DocumentsApi->api_v1_documents_id_retry_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->api_v1_documents_id_retry_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

[**ApiV1DocumentsIdRetryPost202Response**](ApiV1DocumentsIdRetryPost202Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_documents_next_correlativo_get**
> ApiV1DocumentsNextCorrelativoGet200Response api_v1_documents_next_correlativo_get(company_ruc, tipo_doc, serie)

Obtener el siguiente correlativo disponible para una serie

Busca el correlativo más alto existente para la combinación empresa+tipoDoc+serie y retorna el siguiente. Útil para auto-numeración.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_documents_next_correlativo_get200_response import ApiV1DocumentsNextCorrelativoGet200Response
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
    api_instance = intifact_sdk.DocumentsApi(api_client)
    company_ruc = 'company_ruc_example' # str | 
    tipo_doc = 'tipo_doc_example' # str | 
    serie = 'serie_example' # str | 

    try:
        # Obtener el siguiente correlativo disponible para una serie
        api_response = api_instance.api_v1_documents_next_correlativo_get(company_ruc, tipo_doc, serie)
        print("The response of DocumentsApi->api_v1_documents_next_correlativo_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->api_v1_documents_next_correlativo_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **company_ruc** | **str**|  | 
 **tipo_doc** | **str**|  | 
 **serie** | **str**|  | 

### Return type

[**ApiV1DocumentsNextCorrelativoGet200Response**](ApiV1DocumentsNextCorrelativoGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

