# intifact_sdk.CompanyApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_company_logo**](CompanyApi.md#delete_company_logo) | **DELETE** /api/v1/companies/{id}/logo | Eliminar logo de la empresa
[**get_company**](CompanyApi.md#get_company) | **GET** /api/v1/companies/{id} | Detalle de empresa
[**get_company_logo**](CompanyApi.md#get_company_logo) | **GET** /api/v1/companies/{id}/logo | Obtener logo de la empresa (PNG/JPG)
[**list_companies**](CompanyApi.md#list_companies) | **GET** /api/v1/companies | Listar empresas emisoras
[**register_company**](CompanyApi.md#register_company) | **POST** /api/v1/companies/register | Dar de alta una empresa con su certificado digital
[**update_company**](CompanyApi.md#update_company) | **PUT** /api/v1/companies/{id} | Actualizar empresa
[**upload_company_certificate**](CompanyApi.md#upload_company_certificate) | **POST** /api/v1/companies/{id}/certificate | Subir certificado digital (.p12/.pfx en base64)
[**upload_company_logo**](CompanyApi.md#upload_company_logo) | **POST** /api/v1/companies/{id}/logo | Subir logo de la empresa (PNG/JPG, max 200KB)


# **delete_company_logo**
> delete_company_logo(id)

Eliminar logo de la empresa

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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Eliminar logo de la empresa
        api_instance.delete_company_logo(id)
    except Exception as e:
        print("Exception when calling CompanyApi->delete_company_logo: %s\n" % e)
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

# **get_company**
> get_company(id)

Detalle de empresa

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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Detalle de empresa
        api_instance.get_company(id)
    except Exception as e:
        print("Exception when calling CompanyApi->get_company: %s\n" % e)
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

# **get_company_logo**
> get_company_logo(id)

Obtener logo de la empresa (PNG/JPG)

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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Obtener logo de la empresa (PNG/JPG)
        api_instance.get_company_logo(id)
    except Exception as e:
        print("Exception when calling CompanyApi->get_company_logo: %s\n" % e)
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

# **list_companies**
> list_companies()

Listar empresas emisoras

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
    api_instance = intifact_sdk.CompanyApi(api_client)

    try:
        # Listar empresas emisoras
        api_instance.list_companies()
    except Exception as e:
        print("Exception when calling CompanyApi->list_companies: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

# **register_company**
> register_company(register_company_request)

Dar de alta una empresa con su certificado digital

Requiere una API key live de cuenta en un plan pago (autogestión incluida). El certificado (.p12/.pfx en base64) tiene que declarar el mismo RUC; si no, no se crea nada.

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.register_company_request import RegisterCompanyRequest
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
    api_instance = intifact_sdk.CompanyApi(api_client)
    register_company_request = intifact_sdk.RegisterCompanyRequest() # RegisterCompanyRequest | 

    try:
        # Dar de alta una empresa con su certificado digital
        api_instance.register_company(register_company_request)
    except Exception as e:
        print("Exception when calling CompanyApi->register_company: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **register_company_request** | [**RegisterCompanyRequest**](RegisterCompanyRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_company**
> update_company(id, update_company_request)

Actualizar empresa

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.update_company_request import UpdateCompanyRequest
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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    update_company_request = intifact_sdk.UpdateCompanyRequest() # UpdateCompanyRequest | 

    try:
        # Actualizar empresa
        api_instance.update_company(id, update_company_request)
    except Exception as e:
        print("Exception when calling CompanyApi->update_company: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **update_company_request** | [**UpdateCompanyRequest**](UpdateCompanyRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_company_certificate**
> upload_company_certificate(id, upload_company_certificate_request)

Subir certificado digital (.p12/.pfx en base64)

### Example

* Bearer Authentication (apiKey):

```python
import intifact_sdk
from intifact_sdk.models.upload_company_certificate_request import UploadCompanyCertificateRequest
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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    upload_company_certificate_request = intifact_sdk.UploadCompanyCertificateRequest() # UploadCompanyCertificateRequest | 

    try:
        # Subir certificado digital (.p12/.pfx en base64)
        api_instance.upload_company_certificate(id, upload_company_certificate_request)
    except Exception as e:
        print("Exception when calling CompanyApi->upload_company_certificate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **upload_company_certificate_request** | [**UploadCompanyCertificateRequest**](UploadCompanyCertificateRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**429** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_company_logo**
> upload_company_logo(id)

Subir logo de la empresa (PNG/JPG, max 200KB)

El logo aparecerá en los PDFs (A4 y ticket). Reemplaza el anterior.

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
    api_instance = intifact_sdk.CompanyApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Subir logo de la empresa (PNG/JPG, max 200KB)
        api_instance.upload_company_logo(id)
    except Exception as e:
        print("Exception when calling CompanyApi->upload_company_logo: %s\n" % e)
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

