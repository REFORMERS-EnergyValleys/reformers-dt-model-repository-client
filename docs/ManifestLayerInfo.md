# ManifestLayerInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**media_type** | **str** |  | [optional] 
**size** | **int** |  | [optional] 
**digest** | **str** |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.manifest_layer_info import ManifestLayerInfo

# TODO update the JSON string below
json = "{}"
# create an instance of ManifestLayerInfo from a JSON string
manifest_layer_info_instance = ManifestLayerInfo.from_json(json)
# print the JSON string representation of the object
print(ManifestLayerInfo.to_json())

# convert the object into a dict
manifest_layer_info_dict = manifest_layer_info_instance.to_dict()
# create an instance of ManifestLayerInfo from a dict
manifest_layer_info_from_dict = ManifestLayerInfo.from_dict(manifest_layer_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


