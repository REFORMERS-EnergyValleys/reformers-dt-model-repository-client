# RepositorySetting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | A unique identifier for this repository | 
**format** | **str** | Component format held in this repository | 
**type** | **str** | Controls if deployments of and updates to artifacts are allowed | 
**url** | **str** | URL to the repository | 
**online** | **bool** | Whether this repository accepts incoming requests | 

## Example

```python
from reformers_model_repo_client.models.repository_setting import RepositorySetting

# TODO update the JSON string below
json = "{}"
# create an instance of RepositorySetting from a JSON string
repository_setting_instance = RepositorySetting.from_json(json)
# print the JSON string representation of the object
print(RepositorySetting.to_json())

# convert the object into a dict
repository_setting_dict = repository_setting_instance.to_dict()
# create an instance of RepositorySetting from a dict
repository_setting_from_dict = RepositorySetting.from_dict(repository_setting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


