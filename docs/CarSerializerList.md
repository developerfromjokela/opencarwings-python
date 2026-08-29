# CarSerializerList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**vin** | **str** |  | 
**last_connection** | **datetime** |  | [optional] [readonly] 
**nickname** | **str** |  | [optional] 
**ev_info** | [**EVInfo**](EVInfo.md) |  | 
**location** | [**LocationInfo**](LocationInfo.md) |  | 
**carrier** | **str** |  | [optional] 
**signal_level** | **int** |  | [optional] 
**tcu_type** | **str** |  | [optional] 

## Example

```python
from opencarwings_client.models.car_serializer_list import CarSerializerList

# TODO update the JSON string below
json = "{}"
# create an instance of CarSerializerList from a JSON string
car_serializer_list_instance = CarSerializerList.from_json(json)
# print the JSON string representation of the object
print(CarSerializerList.to_json())

# convert the object into a dict
car_serializer_list_dict = car_serializer_list_instance.to_dict()
# create an instance of CarSerializerList from a dict
car_serializer_list_from_dict = CarSerializerList.from_dict(car_serializer_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


