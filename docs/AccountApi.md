# openapi_client.AccountApi

All URIs are relative to *https://opencarwings.viaaq.eu*

Method | HTTP request | Description
------------- | ------------- | -------------
[**account_detail_list**](AccountApi.md#account_detail_list) | **GET** /account/detail/ | 
[**account_pin_create**](AccountApi.md#account_pin_create) | **POST** /account/pin/ | 
[**account_reset_api_key_create**](AccountApi.md#account_reset_api_key_create) | **POST** /account/reset-api-key/ | 


# **account_detail_list**
> AccountDetail account_detail_list()

Get basic account details

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.account_detail import AccountDetail
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
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
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AccountApi(api_client)

    try:
        api_response = api_instance.account_detail_list()
        print("The response of AccountApi->account_detail_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->account_detail_list: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AccountDetail**](AccountDetail.md)

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

# **account_pin_create**
> account_pin_create(data)

Change command PIN, requires OTP code if 2FA is enabled, or old pin if disabled

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.pin_change import PinChange
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
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
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AccountApi(api_client)
    data = openapi_client.PinChange() # PinChange | 

    try:
        api_instance.account_pin_create(data)
    except Exception as e:
        print("Exception when calling AccountApi->account_pin_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**PinChange**](PinChange.md)|  | 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**403** | Invalid OTP Code |  -  |
**401** | Not authorized |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **account_reset_api_key_create**
> account_reset_api_key_create()

Reset API-key. ONLY accessible from web portal!

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://opencarwings.viaaq.eu
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
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
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AccountApi(api_client)

    try:
        api_instance.account_reset_api_key_create()
    except Exception as e:
        print("Exception when calling AccountApi->account_reset_api_key_create: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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
**200** | Reset successfully! |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

