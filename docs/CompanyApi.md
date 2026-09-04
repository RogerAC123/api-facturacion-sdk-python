# intifact_sdk.CompanyApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_companies_claim_post**](CompanyApi.md#api_v1_companies_claim_post) | **POST** /api/v1/companies/claim | Reclamar un RUC registrado por otra cuenta, con su certificado
[**api_v1_companies_get**](CompanyApi.md#api_v1_companies_get) | **GET** /api/v1/companies | Listar empresas emisoras
[**api_v1_companies_id_get**](CompanyApi.md#api_v1_companies_id_get) | **GET** /api/v1/companies/{id} | Detalle de empresa
[**api_v1_companies_id_logo_get**](CompanyApi.md#api_v1_companies_id_logo_get) | **GET** /api/v1/companies/{id}/logo | Obtener logo de la empresa (PNG/JPG)
[**api_v1_companies_id_put**](CompanyApi.md#api_v1_companies_id_put) | **PUT** /api/v1/companies/{id} | Actualizar empresa
[**api_v1_companies_post**](CompanyApi.md#api_v1_companies_post) | **POST** /api/v1/companies | Crear empresa emisora


# **api_v1_companies_claim_post**
> api_v1_companies_claim_post(api_v1_companies_claim_post_request)

Reclamar un RUC registrado por otra cuenta, con su certificado

Prueba de titularidad = certificado digital del RUC. Si la cuenta que lo tiene no acreditó titularidad y no emitió documentos, el RUC pasa a tu cuenta.

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_companies_claim_post_request import ApiV1CompaniesClaimPostRequest
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
    api_instance = intifact_sdk.CompanyApi(api_client)
    api_v1_companies_claim_post_request = intifact_sdk.ApiV1CompaniesClaimPostRequest() # ApiV1CompaniesClaimPostRequest | 

    try:
        # Reclamar un RUC registrado por otra cuenta, con su certificado
        api_instance.api_v1_companies_claim_post(api_v1_companies_claim_post_request)
    except Exception as e:
        print("Exception when calling CompanyApi->api_v1_companies_claim_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_companies_claim_post_request** | [**ApiV1CompaniesClaimPostRequest**](ApiV1CompaniesClaimPostRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_companies_get**
> api_v1_companies_get()

Listar empresas emisoras

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
    api_instance = intifact_sdk.CompanyApi(api_client)

    try:
        # Listar empresas emisoras
        api_instance.api_v1_companies_get()
    except Exception as e:
        print("Exception when calling CompanyApi->api_v1_companies_get: %s\n" % e)
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

# **api_v1_companies_id_get**
> api_v1_companies_id_get(id)

Detalle de empresa

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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Detalle de empresa
        api_instance.api_v1_companies_id_get(id)
    except Exception as e:
        print("Exception when calling CompanyApi->api_v1_companies_id_get: %s\n" % e)
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

# **api_v1_companies_id_logo_get**
> api_v1_companies_id_logo_get(id)

Obtener logo de la empresa (PNG/JPG)

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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Obtener logo de la empresa (PNG/JPG)
        api_instance.api_v1_companies_id_logo_get(id)
    except Exception as e:
        print("Exception when calling CompanyApi->api_v1_companies_id_logo_get: %s\n" % e)
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

# **api_v1_companies_id_put**
> api_v1_companies_id_put(id, api_v1_companies_id_put_request)

Actualizar empresa

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_companies_id_put_request import ApiV1CompaniesIdPutRequest
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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    api_v1_companies_id_put_request = intifact_sdk.ApiV1CompaniesIdPutRequest() # ApiV1CompaniesIdPutRequest | 

    try:
        # Actualizar empresa
        api_instance.api_v1_companies_id_put(id, api_v1_companies_id_put_request)
    except Exception as e:
        print("Exception when calling CompanyApi->api_v1_companies_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **api_v1_companies_id_put_request** | [**ApiV1CompaniesIdPutRequest**](ApiV1CompaniesIdPutRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v1_companies_post**
> api_v1_companies_post(api_v1_companies_post_request)

Crear empresa emisora

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_companies_post_request import ApiV1CompaniesPostRequest
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
    api_instance = intifact_sdk.CompanyApi(api_client)
    api_v1_companies_post_request = intifact_sdk.ApiV1CompaniesPostRequest() # ApiV1CompaniesPostRequest | 

    try:
        # Crear empresa emisora
        api_instance.api_v1_companies_post(api_v1_companies_post_request)
    except Exception as e:
        print("Exception when calling CompanyApi->api_v1_companies_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_companies_post_request** | [**ApiV1CompaniesPostRequest**](ApiV1CompaniesPostRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

