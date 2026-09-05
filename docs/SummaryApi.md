# intifact_sdk.SummaryApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_boleta**](SummaryApi.md#cancel_boleta) | **POST** /api/v1/boleta/cancel | Anular boleta via resumen diario (estado&#x3D;3)
[**cancel_invoice**](SummaryApi.md#cancel_invoice) | **POST** /api/v1/invoice/cancel | Anular factura via comunicación de baja
[**get_ticket_status**](SummaryApi.md#get_ticket_status) | **GET** /api/v1/ticket/{ticket}/status | Consultar estado de ticket asíncrono (SOAP o GRE)
[**send_summary**](SummaryApi.md#send_summary) | **POST** /api/v1/summary/send | Enviar resumen diario de boletas (RC)
[**send_voided**](SummaryApi.md#send_voided) | **POST** /api/v1/voided/send | Enviar comunicación de baja (RA)


# **cancel_boleta**
> SendSummary202Response cancel_boleta(cancel_boleta_request)

Anular boleta via resumen diario (estado=3)

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.cancel_boleta_request import CancelBoletaRequest
from intifact_sdk.models.send_summary202_response import SendSummary202Response
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    cancel_boleta_request = intifact_sdk.CancelBoletaRequest() # CancelBoletaRequest | 

    try:
        # Anular boleta via resumen diario (estado=3)
        api_response = api_instance.cancel_boleta(cancel_boleta_request)
        print("The response of SummaryApi->cancel_boleta:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->cancel_boleta: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cancel_boleta_request** | [**CancelBoletaRequest**](CancelBoletaRequest.md)|  | 

### Return type

[**SendSummary202Response**](SendSummary202Response.md)

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

# **cancel_invoice**
> SendSummary202Response cancel_invoice(cancel_invoice_request)

Anular factura via comunicación de baja

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.cancel_invoice_request import CancelInvoiceRequest
from intifact_sdk.models.send_summary202_response import SendSummary202Response
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    cancel_invoice_request = intifact_sdk.CancelInvoiceRequest() # CancelInvoiceRequest | 

    try:
        # Anular factura via comunicación de baja
        api_response = api_instance.cancel_invoice(cancel_invoice_request)
        print("The response of SummaryApi->cancel_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->cancel_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cancel_invoice_request** | [**CancelInvoiceRequest**](CancelInvoiceRequest.md)|  | 

### Return type

[**SendSummary202Response**](SendSummary202Response.md)

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

# **get_ticket_status**
> GetTicketStatus200Response get_ticket_status(ruc, ticket)

Consultar estado de ticket asíncrono (SOAP o GRE)

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.get_ticket_status200_response import GetTicketStatus200Response
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    ruc = 'ruc_example' # str | 
    ticket = 'ticket_example' # str | 

    try:
        # Consultar estado de ticket asíncrono (SOAP o GRE)
        api_response = api_instance.get_ticket_status(ruc, ticket)
        print("The response of SummaryApi->get_ticket_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->get_ticket_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | 
 **ticket** | **str**|  | 

### Return type

[**GetTicketStatus200Response**](GetTicketStatus200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**202** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_summary**
> SendSummary202Response send_summary(send_summary_request)

Enviar resumen diario de boletas (RC)

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_summary202_response import SendSummary202Response
from intifact_sdk.models.send_summary_request import SendSummaryRequest
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    send_summary_request = intifact_sdk.SendSummaryRequest() # SendSummaryRequest | 

    try:
        # Enviar resumen diario de boletas (RC)
        api_response = api_instance.send_summary(send_summary_request)
        print("The response of SummaryApi->send_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->send_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_summary_request** | [**SendSummaryRequest**](SendSummaryRequest.md)|  | 

### Return type

[**SendSummary202Response**](SendSummary202Response.md)

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

# **send_voided**
> SendSummary202Response send_voided(send_voided_request)

Enviar comunicación de baja (RA)

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.send_summary202_response import SendSummary202Response
from intifact_sdk.models.send_voided_request import SendVoidedRequest
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    send_voided_request = intifact_sdk.SendVoidedRequest() # SendVoidedRequest | 

    try:
        # Enviar comunicación de baja (RA)
        api_response = api_instance.send_voided(send_voided_request)
        print("The response of SummaryApi->send_voided:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->send_voided: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_voided_request** | [**SendVoidedRequest**](SendVoidedRequest.md)|  | 

### Return type

[**SendSummary202Response**](SendSummary202Response.md)

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

