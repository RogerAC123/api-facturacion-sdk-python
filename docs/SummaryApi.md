# intifact_sdk.SummaryApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_boleta_cancel_post**](SummaryApi.md#api_v1_boleta_cancel_post) | **POST** /api/v1/boleta/cancel | Anular boleta via resumen diario (estado&#x3D;3)
[**api_v1_invoice_cancel_post**](SummaryApi.md#api_v1_invoice_cancel_post) | **POST** /api/v1/invoice/cancel | Anular factura via comunicación de baja
[**api_v1_summary_send_post**](SummaryApi.md#api_v1_summary_send_post) | **POST** /api/v1/summary/send | Enviar resumen diario de boletas (RC)
[**api_v1_ticket_ticket_status_get**](SummaryApi.md#api_v1_ticket_ticket_status_get) | **GET** /api/v1/ticket/{ticket}/status | Consultar estado de ticket asíncrono (SOAP o GRE)
[**api_v1_voided_send_post**](SummaryApi.md#api_v1_voided_send_post) | **POST** /api/v1/voided/send | Enviar comunicación de baja (RA)


# **api_v1_boleta_cancel_post**
> ApiV1SummarySendPost202Response api_v1_boleta_cancel_post(api_v1_boleta_cancel_post_request)

Anular boleta via resumen diario (estado=3)

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_boleta_cancel_post_request import ApiV1BoletaCancelPostRequest
from intifact_sdk.models.api_v1_summary_send_post202_response import ApiV1SummarySendPost202Response
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    api_v1_boleta_cancel_post_request = intifact_sdk.ApiV1BoletaCancelPostRequest() # ApiV1BoletaCancelPostRequest | 

    try:
        # Anular boleta via resumen diario (estado=3)
        api_response = api_instance.api_v1_boleta_cancel_post(api_v1_boleta_cancel_post_request)
        print("The response of SummaryApi->api_v1_boleta_cancel_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->api_v1_boleta_cancel_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_boleta_cancel_post_request** | [**ApiV1BoletaCancelPostRequest**](ApiV1BoletaCancelPostRequest.md)|  | 

### Return type

[**ApiV1SummarySendPost202Response**](ApiV1SummarySendPost202Response.md)

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

# **api_v1_invoice_cancel_post**
> ApiV1SummarySendPost202Response api_v1_invoice_cancel_post(api_v1_invoice_cancel_post_request)

Anular factura via comunicación de baja

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_invoice_cancel_post_request import ApiV1InvoiceCancelPostRequest
from intifact_sdk.models.api_v1_summary_send_post202_response import ApiV1SummarySendPost202Response
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    api_v1_invoice_cancel_post_request = intifact_sdk.ApiV1InvoiceCancelPostRequest() # ApiV1InvoiceCancelPostRequest | 

    try:
        # Anular factura via comunicación de baja
        api_response = api_instance.api_v1_invoice_cancel_post(api_v1_invoice_cancel_post_request)
        print("The response of SummaryApi->api_v1_invoice_cancel_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->api_v1_invoice_cancel_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_invoice_cancel_post_request** | [**ApiV1InvoiceCancelPostRequest**](ApiV1InvoiceCancelPostRequest.md)|  | 

### Return type

[**ApiV1SummarySendPost202Response**](ApiV1SummarySendPost202Response.md)

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

# **api_v1_summary_send_post**
> ApiV1SummarySendPost202Response api_v1_summary_send_post(api_v1_summary_send_post_request)

Enviar resumen diario de boletas (RC)

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_summary_send_post202_response import ApiV1SummarySendPost202Response
from intifact_sdk.models.api_v1_summary_send_post_request import ApiV1SummarySendPostRequest
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    api_v1_summary_send_post_request = intifact_sdk.ApiV1SummarySendPostRequest() # ApiV1SummarySendPostRequest | 

    try:
        # Enviar resumen diario de boletas (RC)
        api_response = api_instance.api_v1_summary_send_post(api_v1_summary_send_post_request)
        print("The response of SummaryApi->api_v1_summary_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->api_v1_summary_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_summary_send_post_request** | [**ApiV1SummarySendPostRequest**](ApiV1SummarySendPostRequest.md)|  | 

### Return type

[**ApiV1SummarySendPost202Response**](ApiV1SummarySendPost202Response.md)

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

# **api_v1_ticket_ticket_status_get**
> ApiV1TicketTicketStatusGet200Response api_v1_ticket_ticket_status_get(ruc, ticket)

Consultar estado de ticket asíncrono (SOAP o GRE)

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_ticket_ticket_status_get200_response import ApiV1TicketTicketStatusGet200Response
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    ruc = 'ruc_example' # str | 
    ticket = 'ticket_example' # str | 

    try:
        # Consultar estado de ticket asíncrono (SOAP o GRE)
        api_response = api_instance.api_v1_ticket_ticket_status_get(ruc, ticket)
        print("The response of SummaryApi->api_v1_ticket_ticket_status_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->api_v1_ticket_ticket_status_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | 
 **ticket** | **str**|  | 

### Return type

[**ApiV1TicketTicketStatusGet200Response**](ApiV1TicketTicketStatusGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**202** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_voided_send_post**
> ApiV1SummarySendPost202Response api_v1_voided_send_post(api_v1_voided_send_post_request)

Enviar comunicación de baja (RA)

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_summary_send_post202_response import ApiV1SummarySendPost202Response
from intifact_sdk.models.api_v1_voided_send_post_request import ApiV1VoidedSendPostRequest
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
    api_instance = intifact_sdk.SummaryApi(api_client)
    api_v1_voided_send_post_request = intifact_sdk.ApiV1VoidedSendPostRequest() # ApiV1VoidedSendPostRequest | 

    try:
        # Enviar comunicación de baja (RA)
        api_response = api_instance.api_v1_voided_send_post(api_v1_voided_send_post_request)
        print("The response of SummaryApi->api_v1_voided_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SummaryApi->api_v1_voided_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_voided_send_post_request** | [**ApiV1VoidedSendPostRequest**](ApiV1VoidedSendPostRequest.md)|  | 

### Return type

[**ApiV1SummarySendPost202Response**](ApiV1SummarySendPost202Response.md)

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

