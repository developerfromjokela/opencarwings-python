# openapi_client.ApiApi

All URIs are relative to *https://opencarwings.viaaq.eu*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_probe_location_read**](ApiApi.md#api_probe_location_read) | **GET** /api/probe/location/{vin}/ | 


# **api_probe_location_read**
> api_probe_location_read(vin)

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
    api_instance = openapi_client.ApiApi(api_client)
    vin = 'vin_example' # str | 

    try:
        api_instance.api_probe_location_read(vin)
    except Exception as e:
        print("Exception when calling ApiApi->api_probe_location_read: %s\n" % e)
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
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

