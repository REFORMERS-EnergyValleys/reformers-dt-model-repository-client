# RepositorySearchResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[RepositoryComponentInfo]**](RepositoryComponentInfo.md) |  | [optional] 
**continuation_token** | **str** |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.repository_search_result import RepositorySearchResult

# TODO update the JSON string below
json = "{}"
# create an instance of RepositorySearchResult from a JSON string
repository_search_result_instance = RepositorySearchResult.from_json(json)
# print the JSON string representation of the object
print(RepositorySearchResult.to_json())

# convert the object into a dict
repository_search_result_dict = repository_search_result_instance.to_dict()
# create an instance of RepositorySearchResult from a dict
repository_search_result_from_dict = RepositorySearchResult.from_dict(repository_search_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


