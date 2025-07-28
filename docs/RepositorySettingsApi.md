# reformers_model_repo_client.RepositorySettingsApi

All URIs are relative to *https://reformers-dev.vlab-central.ait.ac.at*

Method | HTTP request | Description
------------- | ------------- | -------------
[**repository_settings**](RepositorySettingsApi.md#repository_settings) | **GET** /service/rest/v1/repositorySettings | Retrieve information about available components in the repository.


# **repository_settings**
> List[RepositorySetting] repository_settings()

Retrieve information about available components in the repository.

### Example

* Basic Authentication (BasicHttpAuthentication):

```python
import reformers_model_repo_client
from reformers_model_repo_client.models.repository_setting import RepositorySetting
from reformers_model_repo_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://reformers-dev.vlab-central.ait.ac.at
# See configuration.py for a list of all supported configuration parameters.
configuration = reformers_model_repo_client.Configuration(
    host = "https://reformers-dev.vlab-central.ait.ac.at"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: BasicHttpAuthentication
configuration = reformers_model_repo_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with reformers_model_repo_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = reformers_model_repo_client.RepositorySettingsApi(api_client)

    try:
        # Retrieve information about available components in the repository.
        api_response = api_instance.repository_settings()
        print("The response of RepositorySettingsApi->repository_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RepositorySettingsApi->repository_settings: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[RepositorySetting]**](RepositorySetting.md)

### Authorization

[BasicHttpAuthentication](../README.md#BasicHttpAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

