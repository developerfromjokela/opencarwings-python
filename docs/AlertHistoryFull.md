# AlertHistoryFull


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**type** | **int** |  | 
**type_display** | **str** |  | 
**timestamp** | **datetime** |  | [optional] [readonly] 
**command_id** | **int** |  | [optional] 
**additional_data** | **str** |  | [optional] 
**car** | [**Car**](Car.md) |  | [optional] 

## Example

```python
from openapi_client.models.alert_history_full import AlertHistoryFull

# TODO update the JSON string below
json = "{}"
# create an instance of AlertHistoryFull from a JSON string
alert_history_full_instance = AlertHistoryFull.from_json(json)
# print the JSON string representation of the object
print(AlertHistoryFull.to_json())

# convert the object into a dict
alert_history_full_dict = alert_history_full_instance.to_dict()
# create an instance of AlertHistoryFull from a dict
alert_history_full_from_dict = AlertHistoryFull.from_dict(alert_history_full_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


