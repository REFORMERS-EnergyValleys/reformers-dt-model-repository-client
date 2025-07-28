# RepositoryComponentInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**repository** | **str** |  | [optional] 
**format** | **str** |  | [optional] 
**group** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**assets** | [**List[AssetInfo]**](AssetInfo.md) |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.repository_component_info import RepositoryComponentInfo

# TODO update the JSON string below
json = "{}"
# create an instance of RepositoryComponentInfo from a JSON string
repository_component_info_instance = RepositoryComponentInfo.from_json(json)
# print the JSON string representation of the object
print(RepositoryComponentInfo.to_json())

# convert the object into a dict
repository_component_info_dict = repository_component_info_instance.to_dict()
# create an instance of RepositoryComponentInfo from a dict
repository_component_info_from_dict = RepositoryComponentInfo.from_dict(repository_component_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


