# ManifestNotFoundErrorsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**detail** | **List[object]** |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.manifest_not_found_errors_inner import ManifestNotFoundErrorsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ManifestNotFoundErrorsInner from a JSON string
manifest_not_found_errors_inner_instance = ManifestNotFoundErrorsInner.from_json(json)
# print the JSON string representation of the object
print(ManifestNotFoundErrorsInner.to_json())

# convert the object into a dict
manifest_not_found_errors_inner_dict = manifest_not_found_errors_inner_instance.to_dict()
# create an instance of ManifestNotFoundErrorsInner from a dict
manifest_not_found_errors_inner_from_dict = ManifestNotFoundErrorsInner.from_dict(manifest_not_found_errors_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


