# intifact_sdk.DespatchApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_despatch_id_cdr_get**](DespatchApi.md#api_v1_despatch_id_cdr_get) | **GET** /api/v1/despatch/{id}/cdr | Descargar CDR (constancia de SUNAT)
[**api_v1_despatch_id_pdf_get**](DespatchApi.md#api_v1_despatch_id_pdf_get) | **GET** /api/v1/despatch/{id}/pdf | Obtener PDF de la guía (A4 oficina, ticket 80mm o 58mm POS)
[**api_v1_despatch_id_xml_get**](DespatchApi.md#api_v1_despatch_id_xml_get) | **GET** /api/v1/despatch/{id}/xml | Descargar XML firmado de la guía
[**api_v1_despatch_send_multi_post**](DespatchApi.md#api_v1_despatch_send_multi_post) | **POST** /api/v1/despatch/send-multi | Enviar múltiples guías de remisión por destino
[**api_v1_despatch_send_post**](DespatchApi.md#api_v1_despatch_send_post) | **POST** /api/v1/despatch/send | Enviar guía de remisión (09) via API GRE REST
[**api_v1_despatch_transportista_send_post**](DespatchApi.md#api_v1_despatch_transportista_send_post) | **POST** /api/v1/despatch-transportista/send | Enviar guía de remisión TRANSPORTISTA (31) via API GRE REST


# **api_v1_despatch_id_cdr_get**
> api_v1_despatch_id_cdr_get(id)

Descargar CDR (constancia de SUNAT)

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
    api_instance = intifact_sdk.DespatchApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar CDR (constancia de SUNAT)
        api_instance.api_v1_despatch_id_cdr_get(id)
    except Exception as e:
        print("Exception when calling DespatchApi->api_v1_despatch_id_cdr_get: %s\n" % e)
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

# **api_v1_despatch_id_pdf_get**
> api_v1_despatch_id_pdf_get(id, format=format)

Obtener PDF de la guía (A4 oficina, ticket 80mm o 58mm POS)

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
    api_instance = intifact_sdk.DespatchApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    format = 'a4' # str |  (optional) (default to 'a4')

    try:
        # Obtener PDF de la guía (A4 oficina, ticket 80mm o 58mm POS)
        api_instance.api_v1_despatch_id_pdf_get(id, format=format)
    except Exception as e:
        print("Exception when calling DespatchApi->api_v1_despatch_id_pdf_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **format** | **str**|  | [optional] [default to &#39;a4&#39;]

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

# **api_v1_despatch_id_xml_get**
> api_v1_despatch_id_xml_get(id)

Descargar XML firmado de la guía

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
    api_instance = intifact_sdk.DespatchApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar XML firmado de la guía
        api_instance.api_v1_despatch_id_xml_get(id)
    except Exception as e:
        print("Exception when calling DespatchApi->api_v1_despatch_id_xml_get: %s\n" % e)
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

# **api_v1_despatch_send_multi_post**
> ApiV1DespatchSendMultiPost202Response api_v1_despatch_send_multi_post(api_v1_despatch_send_multi_post_request)

Enviar múltiples guías de remisión por destino

Recibe datos comunes de transporte + array de destinos. Genera una guía por cada destino con correlativo auto-asignado. Cada guía se encola independientemente para envío a SUNAT GRE.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_despatch_send_multi_post202_response import ApiV1DespatchSendMultiPost202Response
from intifact_sdk.models.api_v1_despatch_send_multi_post_request import ApiV1DespatchSendMultiPostRequest
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
    api_instance = intifact_sdk.DespatchApi(api_client)
    api_v1_despatch_send_multi_post_request = intifact_sdk.ApiV1DespatchSendMultiPostRequest() # ApiV1DespatchSendMultiPostRequest | 

    try:
        # Enviar múltiples guías de remisión por destino
        api_response = api_instance.api_v1_despatch_send_multi_post(api_v1_despatch_send_multi_post_request)
        print("The response of DespatchApi->api_v1_despatch_send_multi_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DespatchApi->api_v1_despatch_send_multi_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_despatch_send_multi_post_request** | [**ApiV1DespatchSendMultiPostRequest**](ApiV1DespatchSendMultiPostRequest.md)|  | 

### Return type

[**ApiV1DespatchSendMultiPost202Response**](ApiV1DespatchSendMultiPost202Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_despatch_send_post**
> ApiV1NoteSendPost202Response api_v1_despatch_send_post(api_v1_despatch_send_post_request)

Enviar guía de remisión (09) via API GRE REST

Genera XML UBL 2.1, firma y encola. El worker obtiene token OAuth2, envía a SUNAT GRE, guarda ticket y luego hace polling de getStatus. Idempotente por (RUC emisor, tipoDoc, serie, correlativo): reenviar el mismo comprobante NO lo duplica. Si ya fue aceptado devuelve el mismo id y hash sin reenviar nada a SUNAT; si sigue en proceso responde 409 (esperá el resultado, no cambies el correlativo). Solo un RECHAZADO exige un correlativo nuevo.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_despatch_send_post_request import ApiV1DespatchSendPostRequest
from intifact_sdk.models.api_v1_note_send_post202_response import ApiV1NoteSendPost202Response
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
    api_instance = intifact_sdk.DespatchApi(api_client)
    api_v1_despatch_send_post_request = intifact_sdk.ApiV1DespatchSendPostRequest() # ApiV1DespatchSendPostRequest | 

    try:
        # Enviar guía de remisión (09) via API GRE REST
        api_response = api_instance.api_v1_despatch_send_post(api_v1_despatch_send_post_request)
        print("The response of DespatchApi->api_v1_despatch_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DespatchApi->api_v1_despatch_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_despatch_send_post_request** | [**ApiV1DespatchSendPostRequest**](ApiV1DespatchSendPostRequest.md)|  | 

### Return type

[**ApiV1NoteSendPost202Response**](ApiV1NoteSendPost202Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |
**409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_despatch_transportista_send_post**
> ApiV1NoteSendPost202Response api_v1_despatch_transportista_send_post(api_v1_despatch_transportista_send_post_request)

Enviar guía de remisión TRANSPORTISTA (31) via API GRE REST

Guía emitida por la empresa de transporte (emisor=transportista). Incluye remitente (dueño de los bienes) y destinatario. Genera XML UBL 2.1, firma y encola para envío a SUNAT GRE.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_despatch_transportista_send_post_request import ApiV1DespatchTransportistaSendPostRequest
from intifact_sdk.models.api_v1_note_send_post202_response import ApiV1NoteSendPost202Response
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
    api_instance = intifact_sdk.DespatchApi(api_client)
    api_v1_despatch_transportista_send_post_request = intifact_sdk.ApiV1DespatchTransportistaSendPostRequest() # ApiV1DespatchTransportistaSendPostRequest | 

    try:
        # Enviar guía de remisión TRANSPORTISTA (31) via API GRE REST
        api_response = api_instance.api_v1_despatch_transportista_send_post(api_v1_despatch_transportista_send_post_request)
        print("The response of DespatchApi->api_v1_despatch_transportista_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DespatchApi->api_v1_despatch_transportista_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_despatch_transportista_send_post_request** | [**ApiV1DespatchTransportistaSendPostRequest**](ApiV1DespatchTransportistaSendPostRequest.md)|  | 

### Return type

[**ApiV1NoteSendPost202Response**](ApiV1NoteSendPost202Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |
**409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

