# CarUpdating


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**send_to_car_location** | [**SendToCarLocation**](SendToCarLocation.md) |  | [optional] 
**send_to_car_location_all** | [**List[SendToCarLocation]**](SendToCarLocation.md) |  | [optional] 
**ev_info** | [**EVInfoUpdating**](EVInfoUpdating.md) |  | [optional] 
**route_plans** | [**List[RoutePlan]**](RoutePlan.md) |  | [optional] 
**favorite_channels** | **object** |  | [optional] 
**custom_channels** | **object** |  | [optional] 

## Example

```python
from openapi_client.models.car_updating import CarUpdating

# TODO update the JSON string below
json = "{}"
# create an instance of CarUpdating from a JSON string
car_updating_instance = CarUpdating.from_json(json)
# print the JSON string representation of the object
print(CarUpdating.to_json())

# convert the object into a dict
car_updating_dict = car_updating_instance.to_dict()
# create an instance of CarUpdating from a dict
car_updating_from_dict = CarUpdating.from_dict(car_updating_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


