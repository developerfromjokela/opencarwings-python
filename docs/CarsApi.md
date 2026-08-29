# opencarwings_client.CarsApi

All URIs are relative to *https://opencarwings.viaaq.eu*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_car_delete**](CarsApi.md#api_car_delete) | **DELETE** /api/car/{vin}/ | 
[**api_car_list**](CarsApi.md#api_car_list) | **GET** /api/car/ | 
[**api_car_partial_update**](CarsApi.md#api_car_partial_update) | **PATCH** /api/car/{vin}/ | 
[**api_car_read**](CarsApi.md#api_car_read) | **GET** /api/car/{vin}/ | 
[**api_car_timers_create**](CarsApi.md#api_car_timers_create) | **POST** /api/car/{vin}/timers/ | 
[**api_car_timers_delete**](CarsApi.md#api_car_timers_delete) | **DELETE** /api/car/{vin}/timers/{id} | 
[**api_car_timers_list**](CarsApi.md#api_car_timers_list) | **GET** /api/car/{vin}/timers/ | 
[**api_car_timers_partial_update**](CarsApi.md#api_car_timers_partial_update) | **PATCH** /api/car/{vin}/timers/{id} | 
[**api_car_timers_read**](CarsApi.md#api_car_timers_read) | **GET** /api/car/{vin}/timers/{id} | 
[**api_car_timers_update**](CarsApi.md#api_car_timers_update) | **PUT** /api/car/{vin}/timers/{id} | 
[**api_car_update**](CarsApi.md#api_car_update) | **PUT** /api/car/{vin}/ | 
[**api_command_create**](CarsApi.md#api_command_create) | **POST** /api/command/{vin}/ | 


# **api_car_delete**
> api_car_delete(vin)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 

    try:
        await api_instance.api_car_delete(vin)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_list**
> List[CarSerializerList] api_car_list()

Retrieve a list of cars

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.car_serializer_list import CarSerializerList
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)

    try:
        api_response = await api_instance.api_car_list()
        print("The response of CarsApi->api_car_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_list: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[CarSerializerList]**](CarSerializerList.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |
**401** | Not authorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_partial_update**
> Car api_car_partial_update(vin, data)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.car import Car
from opencarwings_client.models.car_updating import CarUpdating
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    data = opencarwings_client.CarUpdating() # CarUpdating | 

    try:
        api_response = await api_instance.api_car_partial_update(vin, data)
        print("The response of CarsApi->api_car_partial_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_partial_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **data** | [**CarUpdating**](CarUpdating.md)|  | 

### Return type

[**Car**](Car.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_read**
> Car api_car_read(vin)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.car import Car
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 

    try:
        api_response = await api_instance.api_car_read(vin)
        print("The response of CarsApi->api_car_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 

### Return type

[**Car**](Car.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_timers_create**
> CommandTimerSetting api_car_timers_create(vin, data)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.command_timer_setting import CommandTimerSetting
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    data = opencarwings_client.CommandTimerSetting() # CommandTimerSetting | 

    try:
        api_response = await api_instance.api_car_timers_create(vin, data)
        print("The response of CarsApi->api_car_timers_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_timers_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **data** | [**CommandTimerSetting**](CommandTimerSetting.md)|  | 

### Return type

[**CommandTimerSetting**](CommandTimerSetting.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_timers_delete**
> api_car_timers_delete(vin, id)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    id = 'id_example' # str | 

    try:
        await api_instance.api_car_timers_delete(vin, id)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_timers_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_timers_list**
> List[CommandTimerSetting] api_car_timers_list(vin)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.command_timer_setting import CommandTimerSetting
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 

    try:
        api_response = await api_instance.api_car_timers_list(vin)
        print("The response of CarsApi->api_car_timers_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_timers_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 

### Return type

[**List[CommandTimerSetting]**](CommandTimerSetting.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_timers_partial_update**
> CommandTimerSetting api_car_timers_partial_update(vin, id, data)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.command_timer_setting import CommandTimerSetting
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    id = 'id_example' # str | 
    data = opencarwings_client.CommandTimerSetting() # CommandTimerSetting | 

    try:
        api_response = await api_instance.api_car_timers_partial_update(vin, id, data)
        print("The response of CarsApi->api_car_timers_partial_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_timers_partial_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **id** | **str**|  | 
 **data** | [**CommandTimerSetting**](CommandTimerSetting.md)|  | 

### Return type

[**CommandTimerSetting**](CommandTimerSetting.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_timers_read**
> CommandTimerSetting api_car_timers_read(vin, id)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.command_timer_setting import CommandTimerSetting
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    id = 'id_example' # str | 

    try:
        api_response = await api_instance.api_car_timers_read(vin, id)
        print("The response of CarsApi->api_car_timers_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_timers_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **id** | **str**|  | 

### Return type

[**CommandTimerSetting**](CommandTimerSetting.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_timers_update**
> CommandTimerSetting api_car_timers_update(vin, id, data)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.command_timer_setting import CommandTimerSetting
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    id = 'id_example' # str | 
    data = opencarwings_client.CommandTimerSetting() # CommandTimerSetting | 

    try:
        api_response = await api_instance.api_car_timers_update(vin, id, data)
        print("The response of CarsApi->api_car_timers_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_timers_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **id** | **str**|  | 
 **data** | [**CommandTimerSetting**](CommandTimerSetting.md)|  | 

### Return type

[**CommandTimerSetting**](CommandTimerSetting.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_car_update**
> Car api_car_update(vin, data)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.car import Car
from opencarwings_client.models.car_updating import CarUpdating
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    data = opencarwings_client.CarUpdating() # CarUpdating | 

    try:
        api_response = await api_instance.api_car_update(vin, data)
        print("The response of CarsApi->api_car_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_car_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **data** | [**CarUpdating**](CarUpdating.md)|  | 

### Return type

[**Car**](Car.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_command_create**
> CommandResponse api_command_create(vin, data)

Send a command to your vehicle

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.api_command_create_request import ApiCommandCreateRequest
from opencarwings_client.models.command_response import CommandResponse
from opencarwings_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = opencarwings_client.Configuration(
    host = "https://opencarwings.viaaq.eu"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Bearer
configuration.api_key['Bearer'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Bearer'] = 'Bearer'

# Configure API key authorization: Personal API Key
configuration.api_key['Personal API Key'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Personal API Key'] = 'Bearer'

# Enter a context with an instance of the API client
async with opencarwings_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = opencarwings_client.CarsApi(api_client)
    vin = 'vin_example' # str | 
    data = opencarwings_client.ApiCommandCreateRequest() # ApiCommandCreateRequest | 

    try:
        api_response = await api_instance.api_command_create(vin, data)
        print("The response of CarsApi->api_command_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarsApi->api_command_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 
 **data** | [**ApiCommandCreateRequest**](ApiCommandCreateRequest.md)|  | 

### Return type

[**CommandResponse**](CommandResponse.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |
**403** | Command PIN not set up or invalid |  -  |
**401** | Not authorized |  -  |
**404** | Car not found |  -  |
**400** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

