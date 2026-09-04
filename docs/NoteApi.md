# intifact_sdk.NoteApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_note_compute_post**](NoteApi.md#api_v1_note_compute_post) | **POST** /api/v1/note/compute | Calcular importes (IGV, descuentos, totales) sin emitir
[**api_v1_note_id_cdr_get**](NoteApi.md#api_v1_note_id_cdr_get) | **GET** /api/v1/note/{id}/cdr | Descargar CDR (constancia de SUNAT)
[**api_v1_note_id_pdf_get**](NoteApi.md#api_v1_note_id_pdf_get) | **GET** /api/v1/note/{id}/pdf | Obtener PDF de la nota
[**api_v1_note_id_xml_get**](NoteApi.md#api_v1_note_id_xml_get) | **GET** /api/v1/note/{id}/xml | Descargar XML firmado
[**api_v1_note_send_post**](NoteApi.md#api_v1_note_send_post) | **POST** /api/v1/note/send | Enviar nota de crédito (07) o débito (08) a SUNAT


# **api_v1_note_compute_post**
> ApiV1InvoiceComputePost200Response api_v1_note_compute_post(api_v1_note_compute_post_request)

Calcular importes (IGV, descuentos, totales) sin emitir

Motor de cálculo para notas: recibe ítems crudos (cantidad, valorUnitario sin IGV, afectación, descuento) y un descuento global opcional, y devuelve TODOS los importes fiscales calculados. No emite ni persiste nada — úsalo para previsualizar o para alimentar POST /note/send (agrega tú el documento afectado y el motivo).

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_invoice_compute_post200_response import ApiV1InvoiceComputePost200Response
from intifact_sdk.models.api_v1_note_compute_post_request import ApiV1NoteComputePostRequest
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
    api_instance = intifact_sdk.NoteApi(api_client)
    api_v1_note_compute_post_request = intifact_sdk.ApiV1NoteComputePostRequest() # ApiV1NoteComputePostRequest | 

    try:
        # Calcular importes (IGV, descuentos, totales) sin emitir
        api_response = api_instance.api_v1_note_compute_post(api_v1_note_compute_post_request)
        print("The response of NoteApi->api_v1_note_compute_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NoteApi->api_v1_note_compute_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_note_compute_post_request** | [**ApiV1NoteComputePostRequest**](ApiV1NoteComputePostRequest.md)|  | 

### Return type

[**ApiV1InvoiceComputePost200Response**](ApiV1InvoiceComputePost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_note_id_cdr_get**
> api_v1_note_id_cdr_get(id)

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
    api_instance = intifact_sdk.NoteApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar CDR (constancia de SUNAT)
        api_instance.api_v1_note_id_cdr_get(id)
    except Exception as e:
        print("Exception when calling NoteApi->api_v1_note_id_cdr_get: %s\n" % e)
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

# **api_v1_note_id_pdf_get**
> api_v1_note_id_pdf_get(id)

Obtener PDF de la nota

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
    api_instance = intifact_sdk.NoteApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Obtener PDF de la nota
        api_instance.api_v1_note_id_pdf_get(id)
    except Exception as e:
        print("Exception when calling NoteApi->api_v1_note_id_pdf_get: %s\n" % e)
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

# **api_v1_note_id_xml_get**
> api_v1_note_id_xml_get(id)

Descargar XML firmado

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
    api_instance = intifact_sdk.NoteApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar XML firmado
        api_instance.api_v1_note_id_xml_get(id)
    except Exception as e:
        print("Exception when calling NoteApi->api_v1_note_id_xml_get: %s\n" % e)
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

# **api_v1_note_send_post**
> ApiV1NoteSendPost202Response api_v1_note_send_post(api_v1_note_send_post_request)

Enviar nota de crédito (07) o débito (08) a SUNAT

Genera XML UBL 2.1, firma y encola. Responde 202. Consultar GET /documents/{id} para el resultado final. Idempotente por (RUC emisor, tipoDoc, serie, correlativo): reenviar el mismo comprobante NO lo duplica. Si ya fue aceptado devuelve el mismo id y hash sin reenviar nada a SUNAT; si sigue en proceso responde 409 (esperá el resultado, no cambies el correlativo). Solo un RECHAZADO exige un correlativo nuevo.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_note_send_post202_response import ApiV1NoteSendPost202Response
from intifact_sdk.models.api_v1_note_send_post_request import ApiV1NoteSendPostRequest
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
    api_instance = intifact_sdk.NoteApi(api_client)
    api_v1_note_send_post_request = intifact_sdk.ApiV1NoteSendPostRequest() # ApiV1NoteSendPostRequest | 

    try:
        # Enviar nota de crédito (07) o débito (08) a SUNAT
        api_response = api_instance.api_v1_note_send_post(api_v1_note_send_post_request)
        print("The response of NoteApi->api_v1_note_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NoteApi->api_v1_note_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_note_send_post_request** | [**ApiV1NoteSendPostRequest**](ApiV1NoteSendPostRequest.md)|  | 

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

