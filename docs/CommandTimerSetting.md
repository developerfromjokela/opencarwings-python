# CommandTimerSetting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**command_type_display** | **str** |  | [optional] 
**last_command_result_display** | **str** |  | [optional] 
**timer_type_display** | **str** |  | [optional] 
**last_command_execution** | **datetime** |  | [optional] [readonly] 
**enabled** | **bool** |  | [optional] 
**name** | **str** |  | 
**timer_type** | **int** |  | [optional] 
**command_type** | **int** |  | [optional] 
**last_command_result** | **int** |  | [optional] 
**weekday_mon** | **bool** |  | [optional] 
**weekday_tue** | **bool** |  | [optional] 
**weekday_wed** | **bool** |  | [optional] 
**weekday_thu** | **bool** |  | [optional] 
**weekday_fri** | **bool** |  | [optional] 
**weekday_sat** | **bool** |  | [optional] 
**weekday_sun** | **bool** |  | [optional] 
**time** | **str** |  | 
**var_date** | **date** |  | [optional] 

## Example

```python
from openapi_client.models.command_timer_setting import CommandTimerSetting

# TODO update the JSON string below
json = "{}"
# create an instance of CommandTimerSetting from a JSON string
command_timer_setting_instance = CommandTimerSetting.from_json(json)
# print the JSON string representation of the object
print(CommandTimerSetting.to_json())

# convert the object into a dict
command_timer_setting_dict = command_timer_setting_instance.to_dict()
# create an instance of CommandTimerSetting from a dict
command_timer_setting_from_dict = CommandTimerSetting.from_dict(command_timer_setting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


