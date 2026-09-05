# intifact_sdk.PublicApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**consultar_comprobante**](PublicApi.md#consultar_comprobante) | **GET** /api/v1/public/consultar/{ruc}/{tipoDoc}/{serie}/{numero} | Consultar un comprobante (público, sin auth)
[**consultar_comprobante_pdf**](PublicApi.md#consultar_comprobante_pdf) | **GET** /api/v1/public/consultar/{ruc}/{tipoDoc}/{serie}/{numero}/pdf | Descargar PDF del comprobante (público)
[**consultar_comprobante_xml**](PublicApi.md#consultar_comprobante_xml) | **GET** /api/v1/public/consultar/{ruc}/{tipoDoc}/{serie}/{numero}/xml | Descargar XML firmado (público)


# **consultar_comprobante**
> consultar_comprobante(ruc, tipo_doc, serie, numero, total=total, fecha=fecha, receptor=receptor)

Consultar un comprobante (público, sin auth)

Verificación pública de un comprobante emitido. Retorna datos mínimos no sensibles. El parámetro `total` es opcional pero recomendado como anti-scraping (debe coincidir con el monto total).

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
    api_instance = intifact_sdk.PublicApi(api_client)
    ruc = 'ruc_example' # str | 
    tipo_doc = 'tipo_doc_example' # str | 
    serie = 'serie_example' # str | 
    numero = 'numero_example' # str | 
    total = 3.4 # float |  (optional)
    fecha = 'fecha_example' # str |  (optional)
    receptor = 'receptor_example' # str |  (optional)

    try:
        # Consultar un comprobante (público, sin auth)
        api_instance.consultar_comprobante(ruc, tipo_doc, serie, numero, total=total, fecha=fecha, receptor=receptor)
    except Exception as e:
        print("Exception when calling PublicApi->consultar_comprobante: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | 
 **tipo_doc** | **str**|  | 
 **serie** | **str**|  | 
 **numero** | **str**|  | 
 **total** | **float**|  | [optional] 
 **fecha** | **str**|  | [optional] 
 **receptor** | **str**|  | [optional] 

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

# **consultar_comprobante_pdf**
> consultar_comprobante_pdf(ruc, tipo_doc, serie, numero, total=total, fecha=fecha, receptor=receptor)

Descargar PDF del comprobante (público)

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
    api_instance = intifact_sdk.PublicApi(api_client)
    ruc = 'ruc_example' # str | 
    tipo_doc = 'tipo_doc_example' # str | 
    serie = 'serie_example' # str | 
    numero = 'numero_example' # str | 
    total = 3.4 # float |  (optional)
    fecha = 'fecha_example' # str |  (optional)
    receptor = 'receptor_example' # str |  (optional)

    try:
        # Descargar PDF del comprobante (público)
        api_instance.consultar_comprobante_pdf(ruc, tipo_doc, serie, numero, total=total, fecha=fecha, receptor=receptor)
    except Exception as e:
        print("Exception when calling PublicApi->consultar_comprobante_pdf: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | 
 **tipo_doc** | **str**|  | 
 **serie** | **str**|  | 
 **numero** | **str**|  | 
 **total** | **float**|  | [optional] 
 **fecha** | **str**|  | [optional] 
 **receptor** | **str**|  | [optional] 

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

# **consultar_comprobante_xml**
> consultar_comprobante_xml(ruc, tipo_doc, serie, numero, total=total, fecha=fecha, receptor=receptor)

Descargar XML firmado (público)

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
    api_instance = intifact_sdk.PublicApi(api_client)
    ruc = 'ruc_example' # str | 
    tipo_doc = 'tipo_doc_example' # str | 
    serie = 'serie_example' # str | 
    numero = 'numero_example' # str | 
    total = 3.4 # float |  (optional)
    fecha = 'fecha_example' # str |  (optional)
    receptor = 'receptor_example' # str |  (optional)

    try:
        # Descargar XML firmado (público)
        api_instance.consultar_comprobante_xml(ruc, tipo_doc, serie, numero, total=total, fecha=fecha, receptor=receptor)
    except Exception as e:
        print("Exception when calling PublicApi->consultar_comprobante_xml: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruc** | **str**|  | 
 **tipo_doc** | **str**|  | 
 **serie** | **str**|  | 
 **numero** | **str**|  | 
 **total** | **float**|  | [optional] 
 **fecha** | **str**|  | [optional] 
 **receptor** | **str**|  | [optional] 

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

