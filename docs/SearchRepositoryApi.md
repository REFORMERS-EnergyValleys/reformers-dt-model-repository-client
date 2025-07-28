# reformers_model_repo_client.SearchRepositoryApi

All URIs are relative to *https://reformers-dev.vlab-central.ait.ac.at*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_assets**](SearchRepositoryApi.md#search_assets) | **GET** /service/rest/v1/search/assets | Retrieve information about available assets in the repository.
[**search_components**](SearchRepositoryApi.md#search_components) | **GET** /service/rest/v1/search | Retrieve information about available components in the repository.


# **search_assets**
> RepositorySearchResult search_assets(continuation_token=continuation_token, repository=repository, format=format, group=group, name=name, version=version, docker_image_tag=docker_image_tag, maven_extension=maven_extension)

Retrieve information about available assets in the repository.

### Example


```python
import reformers_model_repo_client
from reformers_model_repo_client.models.repository_search_result import RepositorySearchResult
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

# Enter a context with an instance of the API client
with reformers_model_repo_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = reformers_model_repo_client.SearchRepositoryApi(api_client)
    continuation_token = 'continuation_token_example' # str |  (optional)
    repository = 'repository_example' # str |  (optional)
    format = 'format_example' # str |  (optional)
    group = 'group_example' # str |  (optional)
    name = 'name_example' # str |  (optional)
    version = 'version_example' # str |  (optional)
    docker_image_tag = 'docker_image_tag_example' # str |  (optional)
    maven_extension = 'maven_extension_example' # str |  (optional)

    try:
        # Retrieve information about available assets in the repository.
        api_response = api_instance.search_assets(continuation_token=continuation_token, repository=repository, format=format, group=group, name=name, version=version, docker_image_tag=docker_image_tag, maven_extension=maven_extension)
        print("The response of SearchRepositoryApi->search_assets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchRepositoryApi->search_assets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuation_token** | **str**|  | [optional] 
 **repository** | **str**|  | [optional] 
 **format** | **str**|  | [optional] 
 **group** | **str**|  | [optional] 
 **name** | **str**|  | [optional] 
 **version** | **str**|  | [optional] 
 **docker_image_tag** | **str**|  | [optional] 
 **maven_extension** | **str**|  | [optional] 

### Return type

[**RepositorySearchResult**](RepositorySearchResult.md)

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_components**
> RepositorySearchResult search_components(continuation_token=continuation_token, repository=repository, format=format, group=group, name=name, version=version, docker_image_tag=docker_image_tag, maven_extension=maven_extension)

Retrieve information about available components in the repository.

### Example


```python
import reformers_model_repo_client
from reformers_model_repo_client.models.repository_search_result import RepositorySearchResult
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

# Enter a context with an instance of the API client
with reformers_model_repo_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = reformers_model_repo_client.SearchRepositoryApi(api_client)
    continuation_token = 'continuation_token_example' # str |  (optional)
    repository = 'repository_example' # str |  (optional)
    format = 'format_example' # str |  (optional)
    group = 'group_example' # str |  (optional)
    name = 'name_example' # str |  (optional)
    version = 'version_example' # str |  (optional)
    docker_image_tag = 'docker_image_tag_example' # str |  (optional)
    maven_extension = 'maven_extension_example' # str |  (optional)

    try:
        # Retrieve information about available components in the repository.
        api_response = api_instance.search_components(continuation_token=continuation_token, repository=repository, format=format, group=group, name=name, version=version, docker_image_tag=docker_image_tag, maven_extension=maven_extension)
        print("The response of SearchRepositoryApi->search_components:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchRepositoryApi->search_components: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuation_token** | **str**|  | [optional] 
 **repository** | **str**|  | [optional] 
 **format** | **str**|  | [optional] 
 **group** | **str**|  | [optional] 
 **name** | **str**|  | [optional] 
 **version** | **str**|  | [optional] 
 **docker_image_tag** | **str**|  | [optional] 
 **maven_extension** | **str**|  | [optional] 

### Return type

[**RepositorySearchResult**](RepositorySearchResult.md)

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

