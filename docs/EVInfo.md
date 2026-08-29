# EVInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**last_updated** | **datetime** |  | [optional] [readonly] 
**range_acon** | **int** |  | [optional] 
**range_acoff** | **int** |  | [optional] 
**plugged_in** | **bool** |  | [optional] 
**charging** | **bool** |  | [optional] 
**charge_finish** | **bool** |  | [optional] 
**quick_charging** | **bool** |  | [optional] 
**ac_status** | **bool** |  | [optional] 
**charge_bars** | **int** |  | [optional] 
**car_running** | **bool** |  | [optional] 
**car_gear** | **int** |  | [optional] 
**eco_mode** | **bool** |  | [optional] 
**soh** | **int** |  | [optional] 
**soc** | **float** |  | [optional] 
**soc_display** | **float** |  | [optional] 
**wh_content** | **float** |  | [optional] 
**cap_bars** | **int** |  | [optional] 
**gids** | **int** |  | [optional] 
**counter** | **int** |  | [optional] 
**max_gids** | **int** |  | [optional] 
**full_chg_time** | **int** |  | [optional] 
**limit_chg_time** | **int** |  | [optional] 
**obc_6kw** | **int** |  | [optional] 
**param21** | **int** |  | [optional] 
**cabin_temp** | **float** |  | [optional] 
**force_soc_display** | **bool** |  | [optional] 
**obc_6kw_avail** | **bool** |  | [optional] 
**batt_heater_avail** | **bool** |  | [optional] 
**batt_heater_status** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.ev_info import EVInfo

# TODO update the JSON string below
json = "{}"
# create an instance of EVInfo from a JSON string
ev_info_instance = EVInfo.from_json(json)
# print the JSON string representation of the object
print(EVInfo.to_json())

# convert the object into a dict
ev_info_dict = ev_info_instance.to_dict()
# create an instance of EVInfo from a dict
ev_info_from_dict = EVInfo.from_dict(ev_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


