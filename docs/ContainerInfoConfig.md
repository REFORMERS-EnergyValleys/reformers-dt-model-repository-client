# ContainerInfoConfig


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**env** | **List[str]** |  | [optional] 
**cmd** | **List[str]** |  | [optional] 
**labels** | **Dict[str, str]** |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.container_info_config import ContainerInfoConfig

# TODO update the JSON string below
json = "{}"
# create an instance of ContainerInfoConfig from a JSON string
container_info_config_instance = ContainerInfoConfig.from_json(json)
# print the JSON string representation of the object
print(ContainerInfoConfig.to_json())

# convert the object into a dict
container_info_config_dict = container_info_config_instance.to_dict()
# create an instance of ContainerInfoConfig from a dict
container_info_config_from_dict = ContainerInfoConfig.from_dict(container_info_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


