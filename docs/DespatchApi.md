# intifact_sdk.DespatchApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_despatch_cdr**](DespatchApi.md#get_despatch_cdr) | **GET** /api/v1/despatch/{id}/cdr | Descargar CDR (constancia de SUNAT)
[**get_despatch_pdf**](DespatchApi.md#get_despatch_pdf) | **GET** /api/v1/despatch/{id}/pdf | Obtener PDF de la guía (A4 oficina, ticket 80mm o 58mm POS)
[**get_despatch_xml**](DespatchApi.md#get_despatch_xml) | **GET** /api/v1/despatch/{id}/xml | Descargar XML firmado de la guía
[**send_despatch**](DespatchApi.md#send_despatch) | **POST** /api/v1/despatch/send | Enviar guía de remisión (09) via API GRE REST
[**send_despatch_multi**](DespatchApi.md#send_despatch_multi) | **POST** /api/v1/despatch/send-multi | Enviar múltiples guías de remisión por destino
[**send_despatch_transportista**](DespatchApi.md#send_despatch_transportista) | **POST** /api/v1/despatch-transportista/send | Enviar guía de remisión TRANSPORTISTA (31) via API GRE REST


# **get_despatch_cdr**
> get_despatch_cdr(id)

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
    api_instance = intifact_sdk.DespatchApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar CDR (constancia de SUNAT)
        api_instance.get_despatch_cdr(id)
    except Exception as e:
        print("Exception when calling DespatchApi->get_despatch_cdr: %s\n" % e)
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

# **get_despatch_pdf**
> get_despatch_pdf(id, format=format)

Obtener PDF de la guía (A4 oficina, ticket 80mm o 58mm POS)

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
    api_instance = intifact_sdk.DespatchApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    format = 'a4' # str |  (optional) (default to 'a4')

    try:
        # Obtener PDF de la guía (A4 oficina, ticket 80mm o 58mm POS)
        api_instance.get_despatch_pdf(id, format=format)
    except Exception as e:
        print("Exception when calling DespatchApi->get_despatch_pdf: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **format** | **str**|  | [optional] [default to &#39;a4&#39;]

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

# **get_despatch_xml**
> get_despatch_xml(id)

Descargar XML firmado de la guía

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
    api_instance = intifact_sdk.DespatchApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar XML firmado de la guía
        api_instance.get_despatch_xml(id)
    except Exception as e:
        print("Exception when calling DespatchApi->get_despatch_xml: %s\n" % e)
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

# **send_despatch**
> SendInvoice202Response send_despatch(send_despatch_request)

Enviar guía de remisión (09) via API GRE REST

Genera XML UBL 2.1, firma y encola. El worker obtiene token OAuth2, envía a SUNAT GRE, guarda ticket y luego hace polling de getStatus. Idempotente por (RUC emisor, tipoDoc, serie, correlativo): reenviar el mismo comprobante NO lo duplica. Si ya fue aceptado devuelve el mismo id y hash sin reenviar nada a SUNAT; si sigue en proceso responde 409 (esperá el resultado, no cambies el correlativo). Solo un RECHAZADO exige un correlativo nuevo.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_despatch_request import SendDespatchRequest
from intifact_sdk.models.send_invoice202_response import SendInvoice202Response
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
    api_instance = intifact_sdk.DespatchApi(api_client)
    send_despatch_request = intifact_sdk.SendDespatchRequest() # SendDespatchRequest | 

    try:
        # Enviar guía de remisión (09) via API GRE REST
        api_response = api_instance.send_despatch(send_despatch_request)
        print("The response of DespatchApi->send_despatch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DespatchApi->send_despatch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_despatch_request** | [**SendDespatchRequest**](SendDespatchRequest.md)|  | 

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

# **send_despatch_multi**
> SendDespatchMulti202Response send_despatch_multi(send_despatch_multi_request)

Enviar múltiples guías de remisión por destino

Recibe datos comunes de transporte + array de destinos. Genera una guía por cada destino con correlativo auto-asignado. Cada guía se encola independientemente para envío a SUNAT GRE.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_despatch_multi202_response import SendDespatchMulti202Response
from intifact_sdk.models.send_despatch_multi_request import SendDespatchMultiRequest
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
    api_instance = intifact_sdk.DespatchApi(api_client)
    send_despatch_multi_request = intifact_sdk.SendDespatchMultiRequest() # SendDespatchMultiRequest | 

    try:
        # Enviar múltiples guías de remisión por destino
        api_response = api_instance.send_despatch_multi(send_despatch_multi_request)
        print("The response of DespatchApi->send_despatch_multi:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DespatchApi->send_despatch_multi: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_despatch_multi_request** | [**SendDespatchMultiRequest**](SendDespatchMultiRequest.md)|  | 

### Return type

[**SendDespatchMulti202Response**](SendDespatchMulti202Response.md)

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
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_despatch_transportista**
> SendInvoice202Response send_despatch_transportista(send_despatch_transportista_request)

Enviar guía de remisión TRANSPORTISTA (31) via API GRE REST

Guía emitida por la empresa de transporte (emisor=transportista). Incluye remitente (dueño de los bienes) y destinatario. Genera XML UBL 2.1, firma y encola para envío a SUNAT GRE.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_despatch_transportista_request import SendDespatchTransportistaRequest
from intifact_sdk.models.send_invoice202_response import SendInvoice202Response
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
    api_instance = intifact_sdk.DespatchApi(api_client)
    send_despatch_transportista_request = intifact_sdk.SendDespatchTransportistaRequest() # SendDespatchTransportistaRequest | 

    try:
        # Enviar guía de remisión TRANSPORTISTA (31) via API GRE REST
        api_response = api_instance.send_despatch_transportista(send_despatch_transportista_request)
        print("The response of DespatchApi->send_despatch_transportista:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DespatchApi->send_despatch_transportista: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_despatch_transportista_request** | [**SendDespatchTransportistaRequest**](SendDespatchTransportistaRequest.md)|  | 

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

