# opencarwings_client.AlertsApi

All URIs are relative to *https://opencarwings.viaaq.eu*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_alerts_read**](AlertsApi.md#api_alerts_read) | **GET** /api/alerts/{vin}/ | 


# **api_alerts_read**
> List[AlertHistoryFull] api_alerts_read(vin)

Retrieve a list of alerts for a vehicle

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import opencarwings_client
from opencarwings_client.models.alert_history_full import AlertHistoryFull
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
    api_instance = opencarwings_client.AlertsApi(api_client)
    vin = 'vin_example' # str | 

    try:
        api_response = await api_instance.api_alerts_read(vin)
        print("The response of AlertsApi->api_alerts_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertsApi->api_alerts_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vin** | **str**|  | 

### Return type

[**List[AlertHistoryFull]**](AlertHistoryFull.md)

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
**404** | Car not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

