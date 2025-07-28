# reformers_model_repo_client.RetrieveBlobsApi

All URIs are relative to *https://reformers-dev.vlab-central.ait.ac.at*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_blob_generator**](RetrieveBlobsApi.md#get_blob_generator) | **GET** /repository/model-generators/v2/{generator-name}/blobs/{digest} | Retrieve blob of model generator image from the repository.
[**get_blob_model**](RetrieveBlobsApi.md#get_blob_model) | **GET** /repository/model-images/v2/{generator-name}/{generator-tag}/{model-name}/blobs/{digest} | Retrieve blob of model image from the repository.


# **get_blob_generator**
> ContainerInfo get_blob_generator(generator_name, digest)

Retrieve blob of model generator image from the repository.

### Example


```python
import reformers_model_repo_client
from reformers_model_repo_client.models.container_info import ContainerInfo
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
    api_instance = reformers_model_repo_client.RetrieveBlobsApi(api_client)
    generator_name = 'generator_name_example' # str | 
    digest = 'digest_example' # str | 

    try:
        # Retrieve blob of model generator image from the repository.
        api_response = api_instance.get_blob_generator(generator_name, digest)
        print("The response of RetrieveBlobsApi->get_blob_generator:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetrieveBlobsApi->get_blob_generator: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generator_name** | **str**|  | 
 **digest** | **str**|  | 

### Return type

[**ContainerInfo**](ContainerInfo.md)

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/vnd.docker.container.image.v1+json, application/vnd.docker.image.rootfs.diff.tar.gzip, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_blob_model**
> ContainerInfo get_blob_model(generator_name, generator_tag, model_name, digest)

Retrieve blob of model image from the repository.

### Example


```python
import reformers_model_repo_client
from reformers_model_repo_client.models.container_info import ContainerInfo
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
    api_instance = reformers_model_repo_client.RetrieveBlobsApi(api_client)
    generator_name = 'generator_name_example' # str | 
    generator_tag = 'generator_tag_example' # str | 
    model_name = 'model_name_example' # str | 
    digest = 'digest_example' # str | 

    try:
        # Retrieve blob of model image from the repository.
        api_response = api_instance.get_blob_model(generator_name, generator_tag, model_name, digest)
        print("The response of RetrieveBlobsApi->get_blob_model:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetrieveBlobsApi->get_blob_model: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generator_name** | **str**|  | 
 **generator_tag** | **str**|  | 
 **model_name** | **str**|  | 
 **digest** | **str**|  | 

### Return type

[**ContainerInfo**](ContainerInfo.md)

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/vnd.docker.container.image.v1+json, application/vnd.docker.image.rootfs.diff.tar.gzip, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

