# PinChange


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**otp_code** | **str** |  | [optional] 
**old_pin** | **str** |  | [optional] 
**new_pin** | **str** |  | 
**new_pin_confirm** | **str** |  | 

## Example

```python
from openapi_client.models.pin_change import PinChange

# TODO update the JSON string below
json = "{}"
# create an instance of PinChange from a JSON string
pin_change_instance = PinChange.from_json(json)
# print the JSON string representation of the object
print(PinChange.to_json())

# convert the object into a dict
pin_change_dict = pin_change_instance.to_dict()
# create an instance of PinChange from a dict
pin_change_from_dict = PinChange.from_dict(pin_change_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


