# openapi_client.MaplinkApi

All URIs are relative to *https://opencarwings.viaaq.eu*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_maplink_resolve_create**](MaplinkApi.md#api_maplink_resolve_create) | **POST** /api/maplink/resolve | 


# **api_maplink_resolve_create**
> MapLinkResolverResponse api_maplink_resolve_create(data)

Resolve maps link from Google or Apple into location

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.map_link_resolver_input import MapLinkResolverInput
from openapi_client.models.map_link_resolver_response import MapLinkResolverResponse
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
    api_instance = openapi_client.MaplinkApi(api_client)
    data = openapi_client.MapLinkResolverInput() # MapLinkResolverInput | 

    try:
        api_response = api_instance.api_maplink_resolve_create(data)
        print("The response of MaplinkApi->api_maplink_resolve_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MaplinkApi->api_maplink_resolve_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**MapLinkResolverInput**](MapLinkResolverInput.md)|  | 

### Return type

[**MapLinkResolverResponse**](MapLinkResolverResponse.md)

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

