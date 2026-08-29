# ApiCommandCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**command_type** | **float** |  | 
**command_payload** | **object** |  | [optional] 
**command_pin** | **str** |  | [optional] 

## Example

```python
from opencarwings_client.models.api_command_create_request import ApiCommandCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiCommandCreateRequest from a JSON string
api_command_create_request_instance = ApiCommandCreateRequest.from_json(json)
# print the JSON string representation of the object
print(ApiCommandCreateRequest.to_json())

# convert the object into a dict
api_command_create_request_dict = api_command_create_request_instance.to_dict()
# create an instance of ApiCommandCreateRequest from a dict
api_command_create_request_from_dict = ApiCommandCreateRequest.from_dict(api_command_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


