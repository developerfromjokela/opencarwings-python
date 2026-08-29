# CommandResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | 
**car** | [**Car**](Car.md) |  | 

## Example

```python
from opencarwings_client.models.command_response import CommandResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommandResponse from a JSON string
command_response_instance = CommandResponse.from_json(json)
# print the JSON string representation of the object
print(CommandResponse.to_json())

# convert the object into a dict
command_response_dict = command_response_instance.to_dict()
# create an instance of CommandResponse from a dict
command_response_from_dict = CommandResponse.from_dict(command_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


