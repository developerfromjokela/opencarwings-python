# openapi_client.TokenApi

All URIs are relative to *https://opencarwings.viaaq.eu*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_token_obtain_create**](TokenApi.md#api_token_obtain_create) | **POST** /api/token/obtain/ | 
[**api_token_refresh_create**](TokenApi.md#api_token_refresh_create) | **POST** /api/token/refresh/ | 
[**api_token_signout_create**](TokenApi.md#api_token_signout_create) | **POST** /api/token/signout/ | 
[**api_token_update_create**](TokenApi.md#api_token_update_create) | **POST** /api/token/update/ | 


# **api_token_obtain_create**
> JWTTokenLogin api_token_obtain_create(data)

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.jwt_token_login import JWTTokenLogin
from openapi_client.models.jwt_token_obtain_pair import JWTTokenObtainPair
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
    api_instance = openapi_client.TokenApi(api_client)
    data = openapi_client.JWTTokenObtainPair() # JWTTokenObtainPair | 

    try:
        api_response = api_instance.api_token_obtain_create(data)
        print("The response of TokenApi->api_token_obtain_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokenApi->api_token_obtain_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**JWTTokenObtainPair**](JWTTokenObtainPair.md)|  | 

### Return type

[**JWTTokenLogin**](JWTTokenLogin.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |
**401** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_token_refresh_create**
> TokenRefresh api_token_refresh_create(data)

Takes a refresh type JSON web token and returns an access type JSON web
token if the refresh token is valid.

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.token_refresh import TokenRefresh
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
    api_instance = openapi_client.TokenApi(api_client)
    data = openapi_client.TokenRefresh() # TokenRefresh | 

    try:
        api_response = api_instance.api_token_refresh_create(data)
        print("The response of TokenApi->api_token_refresh_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokenApi->api_token_refresh_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**TokenRefresh**](TokenRefresh.md)|  | 

### Return type

[**TokenRefresh**](TokenRefresh.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_token_signout_create**
> api_token_signout_create(data)

Sign out and invalidate tokens

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.token_blacklist import TokenBlacklist
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
    api_instance = openapi_client.TokenApi(api_client)
    data = openapi_client.TokenBlacklist() # TokenBlacklist | 

    try:
        api_instance.api_token_signout_create(data)
    except Exception as e:
        print("Exception when calling TokenApi->api_token_signout_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**TokenBlacklist**](TokenBlacklist.md)|  | 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully signed out and token revoked |  -  |
**401** | Not authorized |  -  |
**400** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_token_update_create**
> TokenMetadata api_token_update_create(data)

Update token metadata

### Example

* Api Key Authentication (Bearer):
* Api Key Authentication (Personal API Key):

```python
import openapi_client
from openapi_client.models.token_metadata import TokenMetadata
from openapi_client.models.token_metadata_update import TokenMetadataUpdate
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
    api_instance = openapi_client.TokenApi(api_client)
    data = openapi_client.TokenMetadataUpdate() # TokenMetadataUpdate | 

    try:
        api_response = api_instance.api_token_update_create(data)
        print("The response of TokenApi->api_token_update_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokenApi->api_token_update_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**TokenMetadataUpdate**](TokenMetadataUpdate.md)|  | 

### Return type

[**TokenMetadata**](TokenMetadata.md)

### Authorization

[Bearer](../README.md#Bearer), [Personal API Key](../README.md#Personal API Key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |
**401** | Not authorized |  -  |
**400** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

