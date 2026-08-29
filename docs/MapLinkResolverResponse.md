# MapLinkResolverResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** |  | 
**cause** | **str** |  | [optional] 
**location** | [**MapLinkResolvedLocation**](MapLinkResolvedLocation.md) |  | [optional] 

## Example

```python
from opencarwings_client.models.map_link_resolver_response import MapLinkResolverResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MapLinkResolverResponse from a JSON string
map_link_resolver_response_instance = MapLinkResolverResponse.from_json(json)
# print the JSON string representation of the object
print(MapLinkResolverResponse.to_json())

# convert the object into a dict
map_link_resolver_response_dict = map_link_resolver_response_instance.to_dict()
# create an instance of MapLinkResolverResponse from a dict
map_link_resolver_response_from_dict = MapLinkResolverResponse.from_dict(map_link_resolver_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


