# intifact_sdk.AuthApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v1_auth_login_post**](AuthApi.md#api_v1_auth_login_post) | **POST** /api/v1/auth/login | Login email+password
[**api_v1_auth_logout_post**](AuthApi.md#api_v1_auth_logout_post) | **POST** /api/v1/auth/logout | Cerrar sesión actual (revoca refresh)
[**api_v1_auth_me_get**](AuthApi.md#api_v1_auth_me_get) | **GET** /api/v1/auth/me | Datos del usuario actual
[**api_v1_auth_refresh_post**](AuthApi.md#api_v1_auth_refresh_post) | **POST** /api/v1/auth/refresh | Renovar access token con refresh cookie
[**api_v1_auth_sessions_get**](AuthApi.md#api_v1_auth_sessions_get) | **GET** /api/v1/auth/sessions | Lista de sesiones activas del usuario
[**api_v1_auth_sessions_id_delete**](AuthApi.md#api_v1_auth_sessions_id_delete) | **DELETE** /api/v1/auth/sessions/{id} | Revocar una sesión activa por ID
[**api_v1_auth_signup_post**](AuthApi.md#api_v1_auth_signup_post) | **POST** /api/v1/auth/signup | Registro público: crea Tenant + User + sesión
[**api_v1_auth_verify_email_get**](AuthApi.md#api_v1_auth_verify_email_get) | **GET** /api/v1/auth/verify-email | Confirmar email con token (one-time, 24h)
[**api_v1_auth_verify_email_resend_post**](AuthApi.md#api_v1_auth_verify_email_resend_post) | **POST** /api/v1/auth/verify-email/resend | Re-enviar email de verificación al usuario logueado


# **api_v1_auth_login_post**
> api_v1_auth_login_post(api_v1_auth_login_post_request)

Login email+password

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_auth_login_post_request import ApiV1AuthLoginPostRequest
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
    api_instance = intifact_sdk.AuthApi(api_client)
    api_v1_auth_login_post_request = intifact_sdk.ApiV1AuthLoginPostRequest() # ApiV1AuthLoginPostRequest | 

    try:
        # Login email+password
        api_instance.api_v1_auth_login_post(api_v1_auth_login_post_request)
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_login_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_auth_login_post_request** | [**ApiV1AuthLoginPostRequest**](ApiV1AuthLoginPostRequest.md)|  | 

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

# **api_v1_auth_logout_post**
> api_v1_auth_logout_post()

Cerrar sesión actual (revoca refresh)

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Cerrar sesión actual (revoca refresh)
        api_instance.api_v1_auth_logout_post()
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_logout_post: %s\n" % e)
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

# **api_v1_auth_me_get**
> api_v1_auth_me_get()

Datos del usuario actual

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Datos del usuario actual
        api_instance.api_v1_auth_me_get()
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_me_get: %s\n" % e)
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

# **api_v1_auth_refresh_post**
> api_v1_auth_refresh_post()

Renovar access token con refresh cookie

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Renovar access token con refresh cookie
        api_instance.api_v1_auth_refresh_post()
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_refresh_post: %s\n" % e)
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

# **api_v1_auth_sessions_get**
> api_v1_auth_sessions_get()

Lista de sesiones activas del usuario

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Lista de sesiones activas del usuario
        api_instance.api_v1_auth_sessions_get()
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_sessions_get: %s\n" % e)
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

# **api_v1_auth_sessions_id_delete**
> api_v1_auth_sessions_id_delete(id)

Revocar una sesión activa por ID

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
    api_instance = intifact_sdk.AuthApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Revocar una sesión activa por ID
        api_instance.api_v1_auth_sessions_id_delete(id)
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_sessions_id_delete: %s\n" % e)
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

# **api_v1_auth_signup_post**
> api_v1_auth_signup_post(api_v1_auth_signup_post_request)

Registro público: crea Tenant + User + sesión

### Example


```python
import intifact_sdk
from intifact_sdk.models.api_v1_auth_signup_post_request import ApiV1AuthSignupPostRequest
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
    api_instance = intifact_sdk.AuthApi(api_client)
    api_v1_auth_signup_post_request = intifact_sdk.ApiV1AuthSignupPostRequest() # ApiV1AuthSignupPostRequest | 

    try:
        # Registro público: crea Tenant + User + sesión
        api_instance.api_v1_auth_signup_post(api_v1_auth_signup_post_request)
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_signup_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_v1_auth_signup_post_request** | [**ApiV1AuthSignupPostRequest**](ApiV1AuthSignupPostRequest.md)|  | 

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

# **api_v1_auth_verify_email_get**
> api_v1_auth_verify_email_get(token)

Confirmar email con token (one-time, 24h)

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
    api_instance = intifact_sdk.AuthApi(api_client)
    token = 'token_example' # str | 

    try:
        # Confirmar email con token (one-time, 24h)
        api_instance.api_v1_auth_verify_email_get(token)
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_verify_email_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **str**|  | 

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

# **api_v1_auth_verify_email_resend_post**
> api_v1_auth_verify_email_resend_post()

Re-enviar email de verificación al usuario logueado

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Re-enviar email de verificación al usuario logueado
        api_instance.api_v1_auth_verify_email_resend_post()
    except Exception as e:
        print("Exception when calling AuthApi->api_v1_auth_verify_email_resend_post: %s\n" % e)
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

