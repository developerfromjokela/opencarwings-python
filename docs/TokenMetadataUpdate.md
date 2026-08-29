# TokenMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**refresh** | **str** |  | 
**device_type** | **str** |  | [optional] 
**device_os** | **str** |  | [optional] 
**app_version** | **str** |  | [optional] 
**push_notification_key** | **str** |  | [optional] 

## Example

```python
from opencarwings_client.models.token_metadata_update import TokenMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of TokenMetadataUpdate from a JSON string
token_metadata_update_instance = TokenMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(TokenMetadataUpdate.to_json())

# convert the object into a dict
token_metadata_update_dict = token_metadata_update_instance.to_dict()
# create an instance of TokenMetadataUpdate from a dict
token_metadata_update_from_dict = TokenMetadataUpdate.from_dict(token_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


