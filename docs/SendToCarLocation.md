# SendToCarLocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**lat** | **decimal.Decimal** |  | 
**lon** | **decimal.Decimal** |  | 
**name** | **str** |  | 
**created_at** | **datetime** |  | [optional] [readonly] 

## Example

```python
from opencarwings_client.models.send_to_car_location import SendToCarLocation

# TODO update the JSON string below
json = "{}"
# create an instance of SendToCarLocation from a JSON string
send_to_car_location_instance = SendToCarLocation.from_json(json)
# print the JSON string representation of the object
print(SendToCarLocation.to_json())

# convert the object into a dict
send_to_car_location_dict = send_to_car_location_instance.to_dict()
# create an instance of SendToCarLocation from a dict
send_to_car_location_from_dict = SendToCarLocation.from_dict(send_to_car_location_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


