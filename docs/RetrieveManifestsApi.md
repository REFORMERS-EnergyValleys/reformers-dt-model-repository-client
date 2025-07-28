# reformers_model_repo_client.RetrieveManifestsApi

All URIs are relative to *https://reformers-dev.vlab-central.ait.ac.at*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_manifest_generator**](RetrieveManifestsApi.md#get_manifest_generator) | **GET** /repository/model-generators/v2/{generator-name}/manifests/{generator-tag} | Retrieve manifest of model generator image from the repository.
[**get_manifest_model**](RetrieveManifestsApi.md#get_manifest_model) | **GET** /repository/model-images/v2/{generator-name}/{generator-tag}/{model-name}/manifests/{model-tag} | Retrieve manifest of model image from the repository.


# **get_manifest_generator**
> Manifest get_manifest_generator(generator_name, generator_tag)

Retrieve manifest of model generator image from the repository.

### Example


```python
import reformers_model_repo_client
from reformers_model_repo_client.models.manifest import Manifest
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
    api_instance = reformers_model_repo_client.RetrieveManifestsApi(api_client)
    generator_name = 'generator_name_example' # str | 
    generator_tag = 'generator_tag_example' # str | 

    try:
        # Retrieve manifest of model generator image from the repository.
        api_response = api_instance.get_manifest_generator(generator_name, generator_tag)
        print("The response of RetrieveManifestsApi->get_manifest_generator:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetrieveManifestsApi->get_manifest_generator: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generator_name** | **str**|  | 
 **generator_tag** | **str**|  | 

### Return type

[**Manifest**](Manifest.md)

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_manifest_model**
> Manifest get_manifest_model(generator_name, generator_tag, model_name, model_tag)

Retrieve manifest of model image from the repository.

### Example


```python
import reformers_model_repo_client
from reformers_model_repo_client.models.manifest import Manifest
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
    api_instance = reformers_model_repo_client.RetrieveManifestsApi(api_client)
    generator_name = 'generator_name_example' # str | 
    generator_tag = 'generator_tag_example' # str | 
    model_name = 'model_name_example' # str | 
    model_tag = 'model_tag_example' # str | 

    try:
        # Retrieve manifest of model image from the repository.
        api_response = api_instance.get_manifest_model(generator_name, generator_tag, model_name, model_tag)
        print("The response of RetrieveManifestsApi->get_manifest_model:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetrieveManifestsApi->get_manifest_model: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generator_name** | **str**|  | 
 **generator_tag** | **str**|  | 
 **model_name** | **str**|  | 
 **model_tag** | **str**|  | 

### Return type

[**Manifest**](Manifest.md)

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

