# Car


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**tcu_configuration** | [**TCUConfiguration**](TCUConfiguration.md) |  | 
**location** | [**LocationInfo**](LocationInfo.md) |  | 
**ev_info** | [**EVInfo**](EVInfo.md) |  | 
**veh_health** | [**VehicleHealthInfo**](VehicleHealthInfo.md) |  | [optional] 
**send_to_car_location_all** | [**List[SendToCarLocation]**](SendToCarLocation.md) |  | 
**send_to_car_location** | [**SendToCarLocation**](SendToCarLocation.md) |  | [optional] 
**route_plans** | [**List[RoutePlan]**](RoutePlan.md) |  | 
**command_type_display** | **str** |  | 
**command_result_display** | **str** |  | 
**timer_commands** | [**List[CommandTimerSetting]**](CommandTimerSetting.md) |  | 
**command_request_time** | **datetime** |  | [optional] [readonly] 
**last_connection** | **datetime** |  | [optional] [readonly] 
**supported_commands** | **List[int]** |  | [optional] [readonly] 
**sensitive_commands** | **List[int]** |  | [optional] [readonly] 
**command_pin_enforced** | **bool** |  | [optional] [readonly] 
**vin** | **str** |  | 
**nickname** | **str** |  | [optional] 
**sms_config** | **object** |  | 
**color** | **str** |  | [optional] 
**vehicle_code1** | **int** |  | [optional] 
**vehicle_code2** | **int** |  | [optional] 
**vehicle_code3** | **int** |  | [optional] 
**vehicle_code4** | **int** |  | [optional] 
**tcu_model** | **str** |  | [optional] 
**tcu_serial** | **str** |  | [optional] 
**iccid** | **str** |  | [optional] 
**tcu_ver** | **str** |  | [optional] 
**tcu_user** | **str** |  | [optional] 
**tcu_pass** | **str** |  | [optional] 
**disable_auth** | **bool** |  | [optional] 
**periodic_refresh** | **int** |  | [optional] 
**periodic_refresh_running** | **int** |  | [optional] 
**command_id** | **int** |  | [optional] 
**command_result** | **int** |  | [optional] 
**command_requested** | **bool** |  | [optional] 
**command_payload** | **object** |  | [optional] 
**command_type** | **int** |  | [optional] 
**carrier** | **str** |  | [optional] 
**signal_level** | **int** |  | [optional] 
**odometer** | **int** |  | [optional] 
**navi_version** | **str** |  | [optional] 
**map_version** | **str** |  | [optional] 
**tcu_version** | **str** |  | [optional] 
**favorite_channels** | **object** |  | [optional] 
**custom_channels** | **object** |  | [optional] 
**hmac_key** | **str** |  | [optional] 
**tcu_type** | **str** |  | [optional] 
**owner** | **int** |  | 

## Example

```python
from opencarwings_client.models.car import Car

# TODO update the JSON string below
json = "{}"
# create an instance of Car from a JSON string
car_instance = Car.from_json(json)
# print the JSON string representation of the object
print(Car.to_json())

# convert the object into a dict
car_dict = car_instance.to_dict()
# create an instance of Car from a dict
car_from_dict = Car.from_dict(car_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


