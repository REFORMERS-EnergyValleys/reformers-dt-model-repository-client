# reformers_model_repo_client.HandleArtifactsApi

All URIs are relative to *https://reformers-dev.vlab-central.ait.ac.at*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_artifact**](HandleArtifactsApi.md#add_artifact) | **POST** /service/rest/v1/components | Add artifact (to Maven repository).
[**get_artifact**](HandleArtifactsApi.md#get_artifact) | **GET** /repository/model-artifacts/{generator-name}/{generator-tag}/{model-name}/{model-tag}/{file-name}.{file-extension} | Download model artifact (from Maven repository).


# **add_artifact**
> add_artifact(repository, version, maven2_generate_pom=maven2_generate_pom, maven2_group_id=maven2_group_id, maven2_artifact_id=maven2_artifact_id, maven2_asset1=maven2_asset1, maven2_asset1_extension=maven2_asset1_extension, maven2_asset1_classifier=maven2_asset1_classifier, maven2_asset2=maven2_asset2, maven2_asset2_extension=maven2_asset2_extension, maven2_asset2_classifier=maven2_asset2_classifier, maven2_asset3=maven2_asset3, maven2_asset3_extension=maven2_asset3_extension, maven2_asset3_classifier=maven2_asset3_classifier)

Add artifact (to Maven repository).

### Example

* Basic Authentication (BasicHttpAuthentication):

```python
import reformers_model_repo_client
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
    api_instance = reformers_model_repo_client.HandleArtifactsApi(api_client)
    repository = 'repository_example' # str | 
    version = 'version_example' # str | model artifact version
    maven2_generate_pom = True # bool | generate a [POM](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html) file for artifact (optional) (default to True)
    maven2_group_id = 'maven2_group_id_example' # str | group ID (optional)
    maven2_artifact_id = 'maven2_artifact_id_example' # str | artifact ID (optional)
    maven2_asset1 = None # bytearray | artifact \\\\#1 file content (optional)
    maven2_asset1_extension = 'maven2_asset1_extension_example' # str | artifact \\\\#1 file extension (optional)
    maven2_asset1_classifier = 'maven2_asset1_classifier_example' # str | artifact \\\\#1 classifier (optional)
    maven2_asset2 = None # bytearray | artifact \\\\#2 file content (optional)
    maven2_asset2_extension = 'maven2_asset2_extension_example' # str | artifact \\\\#2 file extension (optional)
    maven2_asset2_classifier = 'maven2_asset2_classifier_example' # str | artifact \\\\#2 classifier (optional)
    maven2_asset3 = None # bytearray | artifact \\\\#3 file content (optional)
    maven2_asset3_extension = 'maven2_asset3_extension_example' # str | artifact \\\\#3 file extension (optional)
    maven2_asset3_classifier = 'maven2_asset3_classifier_example' # str | artifact \\\\#3 classifier (optional)

    try:
        # Add artifact (to Maven repository).
        api_instance.add_artifact(repository, version, maven2_generate_pom=maven2_generate_pom, maven2_group_id=maven2_group_id, maven2_artifact_id=maven2_artifact_id, maven2_asset1=maven2_asset1, maven2_asset1_extension=maven2_asset1_extension, maven2_asset1_classifier=maven2_asset1_classifier, maven2_asset2=maven2_asset2, maven2_asset2_extension=maven2_asset2_extension, maven2_asset2_classifier=maven2_asset2_classifier, maven2_asset3=maven2_asset3, maven2_asset3_extension=maven2_asset3_extension, maven2_asset3_classifier=maven2_asset3_classifier)
    except Exception as e:
        print("Exception when calling HandleArtifactsApi->add_artifact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repository** | **str**|  | 
 **version** | **str**| model artifact version | 
 **maven2_generate_pom** | **bool**| generate a [POM](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html) file for artifact | [optional] [default to True]
 **maven2_group_id** | **str**| group ID | [optional] 
 **maven2_artifact_id** | **str**| artifact ID | [optional] 
 **maven2_asset1** | **bytearray**| artifact \\\\#1 file content | [optional] 
 **maven2_asset1_extension** | **str**| artifact \\\\#1 file extension | [optional] 
 **maven2_asset1_classifier** | **str**| artifact \\\\#1 classifier | [optional] 
 **maven2_asset2** | **bytearray**| artifact \\\\#2 file content | [optional] 
 **maven2_asset2_extension** | **str**| artifact \\\\#2 file extension | [optional] 
 **maven2_asset2_classifier** | **str**| artifact \\\\#2 classifier | [optional] 
 **maven2_asset3** | **bytearray**| artifact \\\\#3 file content | [optional] 
 **maven2_asset3_extension** | **str**| artifact \\\\#3 file extension | [optional] 
 **maven2_asset3_classifier** | **str**| artifact \\\\#3 classifier | [optional] 

### Return type

void (empty response body)

### Authorization

[BasicHttpAuthentication](../README.md#BasicHttpAuthentication)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |
**401** | Unauthorized |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_artifact**
> bytearray get_artifact(generator_name, generator_tag, model_name, model_tag, file_name, file_extension)

Download model artifact (from Maven repository).

### Example


```python
import reformers_model_repo_client
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
    api_instance = reformers_model_repo_client.HandleArtifactsApi(api_client)
    generator_name = 'generator_name_example' # str | 
    generator_tag = 'generator_tag_example' # str | 
    model_name = 'model_name_example' # str | 
    model_tag = 'model_tag_example' # str | 
    file_name = 'file_name_example' # str | 
    file_extension = 'file_extension_example' # str | 

    try:
        # Download model artifact (from Maven repository).
        api_response = api_instance.get_artifact(generator_name, generator_tag, model_name, model_tag, file_name, file_extension)
        print("The response of HandleArtifactsApi->get_artifact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HandleArtifactsApi->get_artifact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generator_name** | **str**|  | 
 **generator_tag** | **str**|  | 
 **model_name** | **str**|  | 
 **model_tag** | **str**|  | 
 **file_name** | **str**|  | 
 **file_extension** | **str**|  | 

### Return type

**bytearray**

### Authorization

[NoAuthentication](../README.md#NoAuthentication)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: *, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

