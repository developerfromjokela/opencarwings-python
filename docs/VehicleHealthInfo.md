# VehicleHealthInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**last_updated** | **datetime** |  | [optional] [readonly] 
**dtc_timestamp** | **datetime** |  | [optional] 
**dtc_short** | **object** |  | [optional] 
**dtc_long** | **object** |  | [optional] 
**tpms_light** | **bool** |  | [optional] 
**tpms_fr** | **int** |  | [optional] 
**tpms_fl** | **int** |  | [optional] 
**tpms_rr** | **int** |  | [optional] 
**tpms_rl** | **int** |  | [optional] 
**maintenance_alert** | **bool** |  | [optional] 
**mileage** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.vehicle_health_info import VehicleHealthInfo

# TODO update the JSON string below
json = "{}"
# create an instance of VehicleHealthInfo from a JSON string
vehicle_health_info_instance = VehicleHealthInfo.from_json(json)
# print the JSON string representation of the object
print(VehicleHealthInfo.to_json())

# convert the object into a dict
vehicle_health_info_dict = vehicle_health_info_instance.to_dict()
# create an instance of VehicleHealthInfo from a dict
vehicle_health_info_from_dict = VehicleHealthInfo.from_dict(vehicle_health_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


