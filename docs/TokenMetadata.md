# TokenMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_type** | **str** |  | [optional] 
**device_os** | **str** |  | [optional] 
**app_version** | **str** |  | [optional] 
**push_notification_key** | **str** |  | [optional] 
**user_agent** | **str** |  | [optional] 
**last_used_at** | **datetime** |  | [optional] [readonly] 

## Example

```python
from openapi_client.models.token_metadata import TokenMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of TokenMetadata from a JSON string
token_metadata_instance = TokenMetadata.from_json(json)
# print the JSON string representation of the object
print(TokenMetadata.to_json())

# convert the object into a dict
token_metadata_dict = token_metadata_instance.to_dict()
# create an instance of TokenMetadata from a dict
token_metadata_from_dict = TokenMetadata.from_dict(token_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


