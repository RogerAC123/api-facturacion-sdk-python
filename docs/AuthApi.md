# intifact_sdk.AuthApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_current_user**](AuthApi.md#get_current_user) | **GET** /api/v1/auth/me | Datos del usuario actual
[**list_sessions**](AuthApi.md#list_sessions) | **GET** /api/v1/auth/sessions | Lista de sesiones activas del usuario
[**login**](AuthApi.md#login) | **POST** /api/v1/auth/login | Login email+password
[**logout**](AuthApi.md#logout) | **POST** /api/v1/auth/logout | Cerrar sesión actual (revoca refresh)
[**refresh_token**](AuthApi.md#refresh_token) | **POST** /api/v1/auth/refresh | Renovar access token con refresh cookie
[**resend_verification_email**](AuthApi.md#resend_verification_email) | **POST** /api/v1/auth/verify-email/resend | Re-enviar email de verificación al usuario logueado
[**revoke_session**](AuthApi.md#revoke_session) | **DELETE** /api/v1/auth/sessions/{id} | Revocar una sesión activa por ID
[**signup**](AuthApi.md#signup) | **POST** /api/v1/auth/signup | Registro público: crea Tenant + User + sesión
[**verify_email**](AuthApi.md#verify_email) | **GET** /api/v1/auth/verify-email | Confirmar email con token (one-time, 24h)


# **get_current_user**
> get_current_user()

Datos del usuario actual

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Datos del usuario actual
        api_instance.get_current_user()
    except Exception as e:
        print("Exception when calling AuthApi->get_current_user: %s\n" % e)
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

# **list_sessions**
> list_sessions()

Lista de sesiones activas del usuario

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Lista de sesiones activas del usuario
        api_instance.list_sessions()
    except Exception as e:
        print("Exception when calling AuthApi->list_sessions: %s\n" % e)
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

# **login**
> login(login_request)

Login email+password

### Example


```python
import intifact_sdk
from intifact_sdk.models.login_request import LoginRequest
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
    login_request = intifact_sdk.LoginRequest() # LoginRequest | 

    try:
        # Login email+password
        api_instance.login(login_request)
    except Exception as e:
        print("Exception when calling AuthApi->login: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **login_request** | [**LoginRequest**](LoginRequest.md)|  | 

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

# **logout**
> logout()

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
        api_instance.logout()
    except Exception as e:
        print("Exception when calling AuthApi->logout: %s\n" % e)
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

# **refresh_token**
> refresh_token()

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
        api_instance.refresh_token()
    except Exception as e:
        print("Exception when calling AuthApi->refresh_token: %s\n" % e)
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

# **resend_verification_email**
> resend_verification_email()

Re-enviar email de verificación al usuario logueado

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
    api_instance = intifact_sdk.AuthApi(api_client)

    try:
        # Re-enviar email de verificación al usuario logueado
        api_instance.resend_verification_email()
    except Exception as e:
        print("Exception when calling AuthApi->resend_verification_email: %s\n" % e)
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

# **revoke_session**
> revoke_session(id)

Revocar una sesión activa por ID

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
    api_instance = intifact_sdk.AuthApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Revocar una sesión activa por ID
        api_instance.revoke_session(id)
    except Exception as e:
        print("Exception when calling AuthApi->revoke_session: %s\n" % e)
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

# **signup**
> signup(signup_request)

Registro público: crea Tenant + User + sesión

### Example


```python
import intifact_sdk
from intifact_sdk.models.signup_request import SignupRequest
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
    signup_request = intifact_sdk.SignupRequest() # SignupRequest | 

    try:
        # Registro público: crea Tenant + User + sesión
        api_instance.signup(signup_request)
    except Exception as e:
        print("Exception when calling AuthApi->signup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **signup_request** | [**SignupRequest**](SignupRequest.md)|  | 

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

# **verify_email**
> verify_email(token)

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
        api_instance.verify_email(token)
    except Exception as e:
        print("Exception when calling AuthApi->verify_email: %s\n" % e)
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

