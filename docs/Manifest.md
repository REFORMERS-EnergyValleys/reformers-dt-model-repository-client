# Manifest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**schema_version** | **int** |  | [optional] 
**media_type** | **str** |  | [optional] 
**config** | [**ManifestLayerInfo**](ManifestLayerInfo.md) |  | [optional] 
**layers** | [**List[ManifestLayerInfo]**](ManifestLayerInfo.md) |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.manifest import Manifest

# TODO update the JSON string below
json = "{}"
# create an instance of Manifest from a JSON string
manifest_instance = Manifest.from_json(json)
# print the JSON string representation of the object
print(Manifest.to_json())

# convert the object into a dict
manifest_dict = manifest_instance.to_dict()
# create an instance of Manifest from a dict
manifest_from_dict = Manifest.from_dict(manifest_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


