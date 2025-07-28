# BlobNotFoundErrorsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**detail** | **str** |  | [optional] 

## Example

```python
from reformers_model_repo_client.models.blob_not_found_errors_inner import BlobNotFoundErrorsInner

# TODO update the JSON string below
json = "{}"
# create an instance of BlobNotFoundErrorsInner from a JSON string
blob_not_found_errors_inner_instance = BlobNotFoundErrorsInner.from_json(json)
# print the JSON string representation of the object
print(BlobNotFoundErrorsInner.to_json())

# convert the object into a dict
blob_not_found_errors_inner_dict = blob_not_found_errors_inner_instance.to_dict()
# create an instance of BlobNotFoundErrorsInner from a dict
blob_not_found_errors_inner_from_dict = BlobNotFoundErrorsInner.from_dict(blob_not_found_errors_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


