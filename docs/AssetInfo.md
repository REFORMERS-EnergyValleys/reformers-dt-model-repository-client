# AssetInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**download_url** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**repository** | **str** |  | [optional] 
**format** | **str** |  | [optional] 
**checksum** | **object** |  | [optional] 
**content_type** | **str** |  | [optional] 
**last_modified** | **str** |  | [optional] 
**last_downloaded** | **str** |  | [optional] 
**uploader** | **str** |  | [optional] 
**uploader_ip** | **str** |  | [optional] 
**file_size** | **int** |  | [optional] 
**blob_created** | **str** |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.asset_info import AssetInfo

# TODO update the JSON string below
json = "{}"
# create an instance of AssetInfo from a JSON string
asset_info_instance = AssetInfo.from_json(json)
# print the JSON string representation of the object
print(AssetInfo.to_json())

# convert the object into a dict
asset_info_dict = asset_info_instance.to_dict()
# create an instance of AssetInfo from a dict
asset_info_from_dict = AssetInfo.from_dict(asset_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


