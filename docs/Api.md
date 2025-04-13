# openapi_client.Api

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoice_create_wallet_post**](Api.md#invoice_create_wallet_post) | **POST** /invoice/create/wallet | Создание статического кошелька


# **invoice_create_wallet_post**
> InlineResponse200 invoice_create_wallet_post(x_api_key=x_api_key, inline_object=inline_object)

Создание статического кошелька

### Example

```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.Api(api_client)
    x_api_key = 'x_api_key_example' # str | API ключ мерчанта (optional)
inline_object = openapi_client.InlineObject() # InlineObject |  (optional)

    try:
        # Создание статического кошелька
        api_response = api_instance.invoice_create_wallet_post(x_api_key=x_api_key, inline_object=inline_object)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->invoice_create_wallet_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_api_key** | **str**| API ключ мерчанта | [optional] 
 **inline_object** | [**InlineObject**](InlineObject.md)|  | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

