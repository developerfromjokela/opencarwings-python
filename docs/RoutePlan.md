# RoutePlan


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**name** | **str** |  | 
**created_at** | **datetime** |  | [optional] [readonly] 
**start_name** | **str** |  | 
**start_lat** | **decimal.Decimal** |  | 
**start_lon** | **decimal.Decimal** |  | 
**finish_name** | **str** |  | 
**finish_lat** | **decimal.Decimal** |  | 
**finish_lon** | **decimal.Decimal** |  | 
**point1_name** | **str** |  | [optional] 
**point1_lat** | **decimal.Decimal** |  | [optional] 
**point1_lon** | **decimal.Decimal** |  | [optional] 
**point2_name** | **str** |  | [optional] 
**point2_lat** | **decimal.Decimal** |  | [optional] 
**point2_lon** | **decimal.Decimal** |  | [optional] 
**point3_name** | **str** |  | [optional] 
**point3_lat** | **decimal.Decimal** |  | [optional] 
**point3_lon** | **decimal.Decimal** |  | [optional] 
**point4_name** | **str** |  | [optional] 
**point4_lat** | **decimal.Decimal** |  | [optional] 
**point4_lon** | **decimal.Decimal** |  | [optional] 
**point5_name** | **str** |  | [optional] 
**point5_lat** | **decimal.Decimal** |  | [optional] 
**point5_lon** | **decimal.Decimal** |  | [optional] 

## Example

```python
from opencarwings_client.models.route_plan import RoutePlan

# TODO update the JSON string below
json = "{}"
# create an instance of RoutePlan from a JSON string
route_plan_instance = RoutePlan.from_json(json)
# print the JSON string representation of the object
print(RoutePlan.to_json())

# convert the object into a dict
route_plan_dict = route_plan_instance.to_dict()
# create an instance of RoutePlan from a dict
route_plan_from_dict = RoutePlan.from_dict(route_plan_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


