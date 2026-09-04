# intifact_sdk.BranchesApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_companies_id_branches_branch_id_delete**](BranchesApi.md#api_v1_companies_id_branches_branch_id_delete) | **DELETE** /api/v1/companies/{id}/branches/{branchId} | Desactivar establecimiento (soft-delete)
[**api_v1_companies_id_branches_branch_id_put**](BranchesApi.md#api_v1_companies_id_branches_branch_id_put) | **PUT** /api/v1/companies/{id}/branches/{branchId} | Actualizar establecimiento
[**api_v1_companies_id_branches_get**](BranchesApi.md#api_v1_companies_id_branches_get) | **GET** /api/v1/companies/{id}/branches | Listar establecimientos (sucursales) de una empresa
[**api_v1_companies_id_branches_post**](BranchesApi.md#api_v1_companies_id_branches_post) | **POST** /api/v1/companies/{id}/branches | Crear establecimiento (sucursal)


# **api_v1_companies_id_branches_branch_id_delete**
> api_v1_companies_id_branches_branch_id_delete(id, branch_id)

Desactivar establecimiento (soft-delete)

No se elimina físicamente porque puede haber documentos emitidos desde ahí. Solo se desactiva (isActive=false).

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
    api_instance = intifact_sdk.BranchesApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    branch_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Desactivar establecimiento (soft-delete)
        api_instance.api_v1_companies_id_branches_branch_id_delete(id, branch_id)
    except Exception as e:
        print("Exception when calling BranchesApi->api_v1_companies_id_branches_branch_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **branch_id** | **UUID**|  | 

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

# **api_v1_companies_id_branches_branch_id_put**
> api_v1_companies_id_branches_branch_id_put(id, branch_id, api_v1_companies_id_branches_branch_id_put_request)

Actualizar establecimiento

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_companies_id_branches_branch_id_put_request import ApiV1CompaniesIdBranchesBranchIdPutRequest
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
    api_instance = intifact_sdk.BranchesApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    branch_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    api_v1_companies_id_branches_branch_id_put_request = intifact_sdk.ApiV1CompaniesIdBranchesBranchIdPutRequest() # ApiV1CompaniesIdBranchesBranchIdPutRequest | 

    try:
        # Actualizar establecimiento
        api_instance.api_v1_companies_id_branches_branch_id_put(id, branch_id, api_v1_companies_id_branches_branch_id_put_request)
    except Exception as e:
        print("Exception when calling BranchesApi->api_v1_companies_id_branches_branch_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **branch_id** | **UUID**|  | 
 **api_v1_companies_id_branches_branch_id_put_request** | [**ApiV1CompaniesIdBranchesBranchIdPutRequest**](ApiV1CompaniesIdBranchesBranchIdPutRequest.md)|  | 

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

# **api_v1_companies_id_branches_get**
> api_v1_companies_id_branches_get(id)

Listar establecimientos (sucursales) de una empresa

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
    api_instance = intifact_sdk.BranchesApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Listar establecimientos (sucursales) de una empresa
        api_instance.api_v1_companies_id_branches_get(id)
    except Exception as e:
        print("Exception when calling BranchesApi->api_v1_companies_id_branches_get: %s\n" % e)
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

# **api_v1_companies_id_branches_post**
> api_v1_companies_id_branches_post(id, api_v1_companies_id_branches_post_request)

Crear establecimiento (sucursal)

El código debe coincidir con el que SUNAT asignó a la sucursal al registrarla en el portal SOL (Mis Trámites > Establecimientos Anexos).

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_companies_id_branches_post_request import ApiV1CompaniesIdBranchesPostRequest
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
    api_instance = intifact_sdk.BranchesApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    api_v1_companies_id_branches_post_request = intifact_sdk.ApiV1CompaniesIdBranchesPostRequest() # ApiV1CompaniesIdBranchesPostRequest | 

    try:
        # Crear establecimiento (sucursal)
        api_instance.api_v1_companies_id_branches_post(id, api_v1_companies_id_branches_post_request)
    except Exception as e:
        print("Exception when calling BranchesApi->api_v1_companies_id_branches_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **api_v1_companies_id_branches_post_request** | [**ApiV1CompaniesIdBranchesPostRequest**](ApiV1CompaniesIdBranchesPostRequest.md)|  | 

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

