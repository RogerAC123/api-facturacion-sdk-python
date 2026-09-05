# intifact_sdk.InvoiceApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**compute_invoice**](InvoiceApi.md#compute_invoice) | **POST** /api/v1/invoice/compute | Calcular importes (IGV, descuentos, totales) sin emitir
[**get_invoice_cdr**](InvoiceApi.md#get_invoice_cdr) | **GET** /api/v1/invoice/{id}/cdr | Descargar CDR (constancia de SUNAT)
[**get_invoice_pdf**](InvoiceApi.md#get_invoice_pdf) | **GET** /api/v1/invoice/{id}/pdf | Obtener PDF (A4 oficina, ticket 80mm o ticket 58mm POS)
[**get_invoice_xml**](InvoiceApi.md#get_invoice_xml) | **GET** /api/v1/invoice/{id}/xml | Descargar XML firmado
[**send_invoice**](InvoiceApi.md#send_invoice) | **POST** /api/v1/invoice/send | Enviar factura (01) o boleta (03) a SUNAT


# **compute_invoice**
> ComputeInvoice200Response compute_invoice(compute_invoice_request)

Calcular importes (IGV, descuentos, totales) sin emitir

Motor de cálculo: recibe ítems crudos (cantidad, valorUnitario sin IGV, afectación, descuento) y un descuento global opcional, y devuelve TODOS los importes fiscales calculados (bases, IGV, descuentos, totales, monto en letras). No emite ni persiste nada — úsalo para previsualizar o para alimentar POST /invoice/send.

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
    api_instance = intifact_sdk.InvoiceApi(api_client)
    compute_invoice_request = intifact_sdk.ComputeInvoiceRequest() # ComputeInvoiceRequest | 

    try:
        # Calcular importes (IGV, descuentos, totales) sin emitir
        api_response = api_instance.compute_invoice(compute_invoice_request)
        print("The response of InvoiceApi->compute_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceApi->compute_invoice: %s\n" % e)
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

# **get_invoice_cdr**
> get_invoice_cdr(id)

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
    api_instance = intifact_sdk.InvoiceApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar CDR (constancia de SUNAT)
        api_instance.get_invoice_cdr(id)
    except Exception as e:
        print("Exception when calling InvoiceApi->get_invoice_cdr: %s\n" % e)
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

# **get_invoice_pdf**
> get_invoice_pdf(id, format=format)

Obtener PDF (A4 oficina, ticket 80mm o ticket 58mm POS)

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
    api_instance = intifact_sdk.InvoiceApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    format = 'a4' # str |  (optional) (default to 'a4')

    try:
        # Obtener PDF (A4 oficina, ticket 80mm o ticket 58mm POS)
        api_instance.get_invoice_pdf(id, format=format)
    except Exception as e:
        print("Exception when calling InvoiceApi->get_invoice_pdf: %s\n" % e)
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

# **get_invoice_xml**
> get_invoice_xml(id)

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
    api_instance = intifact_sdk.InvoiceApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Descargar XML firmado
        api_instance.get_invoice_xml(id)
    except Exception as e:
        print("Exception when calling InvoiceApi->get_invoice_xml: %s\n" % e)
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

# **send_invoice**
> SendInvoice202Response send_invoice(send_invoice_request)

Enviar factura (01) o boleta (03) a SUNAT

Genera el XML UBL 2.1, lo firma digitalmente y lo encola para envío asíncrono a SUNAT. Responde 202 inmediatamente. Para conocer el resultado final consultar GET /documents/{id}. Idempotente por (RUC emisor, tipoDoc, serie, correlativo): reenviar el mismo comprobante NO lo duplica. Si ya fue aceptado devuelve el mismo id y hash sin reenviar nada a SUNAT; si sigue en proceso responde 409 (esperá el resultado, no cambies el correlativo). Solo un RECHAZADO exige un correlativo nuevo.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_invoice202_response import SendInvoice202Response
from intifact_sdk.models.send_invoice_request import SendInvoiceRequest
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
    api_instance = intifact_sdk.InvoiceApi(api_client)
    send_invoice_request = intifact_sdk.SendInvoiceRequest() # SendInvoiceRequest | 

    try:
        # Enviar factura (01) o boleta (03) a SUNAT
        api_response = api_instance.send_invoice(send_invoice_request)
        print("The response of InvoiceApi->send_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceApi->send_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_invoice_request** | [**SendInvoiceRequest**](SendInvoiceRequest.md)|  | 

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

