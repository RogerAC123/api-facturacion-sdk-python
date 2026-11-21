# intifact_sdk.NoteApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**compute_note**](NoteApi.md#compute_note) | **POST** /api/v1/note/compute | Calcular importes (IGV, descuentos, totales) sin emitir
[**get_note_cdr**](NoteApi.md#get_note_cdr) | **GET** /api/v1/note/{id}/cdr | Descargar CDR (constancia de SUNAT)
[**get_note_pdf**](NoteApi.md#get_note_pdf) | **GET** /api/v1/note/{id}/pdf | Obtener PDF de la nota
[**get_note_xml**](NoteApi.md#get_note_xml) | **GET** /api/v1/note/{id}/xml | Descargar XML firmado
[**send_note**](NoteApi.md#send_note) | **POST** /api/v1/note/send | Enviar nota de crédito (07) o débito (08) a SUNAT


# **compute_note**
> ComputeInvoice200Response compute_note(compute_invoice_request)

Calcular importes (IGV, descuentos, totales) sin emitir

Motor de cálculo para notas: recibe ítems crudos (cantidad, valorUnitario sin IGV, afectación, descuento) y un descuento global opcional, y devuelve TODOS los importes fiscales calculados. No emite ni persiste nada — úsalo para previsualizar o para alimentar POST /note/send (agrega tú el documento afectado y el motivo).

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.compute_invoice200_response import ComputeInvoice200Response
from intifact_sdk.models.compute_invoice_request import ComputeInvoiceRequest
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
    api_instance = intifact_sdk.NoteApi(api_client)
    compute_invoice_request = intifact_sdk.ComputeInvoiceRequest() # ComputeInvoiceRequest | 

    try:
        # Calcular importes (IGV, descuentos, totales) sin emitir
        api_response = api_instance.compute_note(compute_invoice_request)
        print("The response of NoteApi->compute_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NoteApi->compute_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compute_invoice_request** | [**ComputeInvoiceRequest**](ComputeInvoiceRequest.md)|  | 

### Return type

[**ComputeInvoice200Response**](ComputeInvoice200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_note_cdr**
> get_note_cdr(id)

Descargar CDR (constancia de SUNAT)

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
    api_instance = intifact_sdk.NoteApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar CDR (constancia de SUNAT)
        api_instance.get_note_cdr(id)
    except Exception as e:
        print("Exception when calling NoteApi->get_note_cdr: %s\n" % e)
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

# **get_note_pdf**
> get_note_pdf(id)

Obtener PDF de la nota

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
    api_instance = intifact_sdk.NoteApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Obtener PDF de la nota
        api_instance.get_note_pdf(id)
    except Exception as e:
        print("Exception when calling NoteApi->get_note_pdf: %s\n" % e)
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

# **get_note_xml**
> get_note_xml(id)

Descargar XML firmado

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
    api_instance = intifact_sdk.NoteApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar XML firmado
        api_instance.get_note_xml(id)
    except Exception as e:
        print("Exception when calling NoteApi->get_note_xml: %s\n" % e)
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

# **send_note**
> SendInvoice202Response send_note(send_note_request)

Enviar nota de crédito (07) o débito (08) a SUNAT

Genera XML UBL 2.1, firma y encola. Responde 202. Consultar GET /documents/{id} para el resultado final. Idempotente por (RUC emisor, tipoDoc, serie, correlativo): reenviar el mismo comprobante NO lo duplica. Si ya fue aceptado devuelve el mismo id y hash sin reenviar nada a SUNAT; si sigue en proceso responde 409 (esperá el resultado, no cambies el correlativo). Solo un RECHAZADO exige un correlativo nuevo.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_invoice202_response import SendInvoice202Response
from intifact_sdk.models.send_note_request import SendNoteRequest
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
    api_instance = intifact_sdk.NoteApi(api_client)
    send_note_request = intifact_sdk.SendNoteRequest() # SendNoteRequest | 

    try:
        # Enviar nota de crédito (07) o débito (08) a SUNAT
        api_response = api_instance.send_note(send_note_request)
        print("The response of NoteApi->send_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NoteApi->send_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_note_request** | [**SendNoteRequest**](SendNoteRequest.md)|  | 

### Return type

[**SendInvoice202Response**](SendInvoice202Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Default Response |  -  |
**400** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**409** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

