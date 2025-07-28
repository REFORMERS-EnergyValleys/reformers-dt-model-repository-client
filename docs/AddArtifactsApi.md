# reformers_model_repo_client.AddArtifactsApi

All URIs are relative to *https://reformers-dev.vlab-central.ait.ac.at*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_component**](AddArtifactsApi.md#add_component) | **POST** /service/rest/v1/components | Add component (to Maven repository).


# **add_component**
> add_component(repository, version, maven2_generate_pom=maven2_generate_pom, maven2_group_id=maven2_group_id, maven2_artifact_id=maven2_artifact_id, maven2_asset1=maven2_asset1, maven2_asset1_extension=maven2_asset1_extension, maven2_asset2=maven2_asset2, maven2_asset2_extension=maven2_asset2_extension, maven2_asset3=maven2_asset3, maven2_asset3_extension=maven2_asset3_extension)

Add component (to Maven repository).

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
    api_instance = reformers_model_repo_client.AddArtifactsApi(api_client)
    repository = 'repository_example' # str | 
    version = 'version_example' # str | 
    maven2_generate_pom = True # bool |  (optional)
    maven2_group_id = 'maven2_group_id_example' # str |  (optional)
    maven2_artifact_id = 'maven2_artifact_id_example' # str |  (optional)
    maven2_asset1 = None # bytearray |  (optional)
    maven2_asset1_extension = 'maven2_asset1_extension_example' # str |  (optional)
    maven2_asset2 = None # bytearray |  (optional)
    maven2_asset2_extension = 'maven2_asset2_extension_example' # str |  (optional)
    maven2_asset3 = None # bytearray |  (optional)
    maven2_asset3_extension = 'maven2_asset3_extension_example' # str |  (optional)

    try:
        # Add component (to Maven repository).
        api_instance.add_component(repository, version, maven2_generate_pom=maven2_generate_pom, maven2_group_id=maven2_group_id, maven2_artifact_id=maven2_artifact_id, maven2_asset1=maven2_asset1, maven2_asset1_extension=maven2_asset1_extension, maven2_asset2=maven2_asset2, maven2_asset2_extension=maven2_asset2_extension, maven2_asset3=maven2_asset3, maven2_asset3_extension=maven2_asset3_extension)
    except Exception as e:
        print("Exception when calling AddArtifactsApi->add_component: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repository** | **str**|  | 
 **version** | **str**|  | 
 **maven2_generate_pom** | **bool**|  | [optional] 
 **maven2_group_id** | **str**|  | [optional] 
 **maven2_artifact_id** | **str**|  | [optional] 
 **maven2_asset1** | **bytearray**|  | [optional] 
 **maven2_asset1_extension** | **str**|  | [optional] 
 **maven2_asset2** | **bytearray**|  | [optional] 
 **maven2_asset2_extension** | **str**|  | [optional] 
 **maven2_asset3** | **bytearray**|  | [optional] 
 **maven2_asset3_extension** | **str**|  | [optional] 

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

