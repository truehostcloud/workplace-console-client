# workplace_client.GetTokenApi

All URIs are relative to *https://workplace-console.truehost.cloud/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_token_create**](GetTokenApi.md#get_token_create) | **POST** /get-token/ | Obtain authentication token


# **get_token_create**
> TokenObtainPair get_token_create(token_obtain_pair)

Obtain authentication token

Takes a set of user credentials and returns an access and refresh JSON web
token pair to prove the authentication of those credentials.

### Example

* Bearer (JWT) Authentication (BearerAuth):

```python
import workplace_client
from workplace_client.models.token_obtain_pair import TokenObtainPair
from workplace_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://workplace-console.truehost.cloud/api
# See configuration.py for a list of all supported configuration parameters.
configuration = workplace_client.Configuration(
    host = "https://workplace-console.truehost.cloud/api"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): BearerAuth
configuration = workplace_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with workplace_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = workplace_client.GetTokenApi(api_client)
    token_obtain_pair = workplace_client.TokenObtainPair() # TokenObtainPair | 

    try:
        # Obtain authentication token
        api_response = api_instance.get_token_create(token_obtain_pair)
        print("The response of GetTokenApi->get_token_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GetTokenApi->get_token_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token_obtain_pair** | [**TokenObtainPair**](TokenObtainPair.md)|  | 

### Return type

[**TokenObtainPair**](TokenObtainPair.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Token pair created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

