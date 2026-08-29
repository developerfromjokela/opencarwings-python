# MapLinkResolvedLocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**lat** | **decimal.Decimal** |  | 
**lon** | **decimal.Decimal** |  | 
**name** | **str** |  | 
**address** | **str** |  | 

## Example

```python
from openapi_client.models.map_link_resolved_location import MapLinkResolvedLocation

# TODO update the JSON string below
json = "{}"
# create an instance of MapLinkResolvedLocation from a JSON string
map_link_resolved_location_instance = MapLinkResolvedLocation.from_json(json)
# print the JSON string representation of the object
print(MapLinkResolvedLocation.to_json())

# convert the object into a dict
map_link_resolved_location_dict = map_link_resolved_location_instance.to_dict()
# create an instance of MapLinkResolvedLocation from a dict
map_link_resolved_location_from_dict = MapLinkResolvedLocation.from_dict(map_link_resolved_location_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


