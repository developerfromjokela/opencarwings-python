# TCUConfiguration


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**last_updated** | **datetime** |  | [optional] [readonly] 
**dial_code** | **str** |  | [optional] 
**apn** | **str** |  | [optional] 
**apn_user** | **str** |  | [optional] 
**apn_password** | **str** |  | [optional] 
**dns1** | **str** |  | [optional] 
**dns2** | **str** |  | [optional] 
**server_url** | **str** |  | [optional] 
**proxy_url** | **str** |  | [optional] 
**connection_type** | **str** |  | [optional] 
**ficosa_config** | **object** |  | [optional] 

## Example

```python
from opencarwings_client.models.tcu_configuration import TCUConfiguration

# TODO update the JSON string below
json = "{}"
# create an instance of TCUConfiguration from a JSON string
tcu_configuration_instance = TCUConfiguration.from_json(json)
# print the JSON string representation of the object
print(TCUConfiguration.to_json())

# convert the object into a dict
tcu_configuration_dict = tcu_configuration_instance.to_dict()
# create an instance of TCUConfiguration from a dict
tcu_configuration_from_dict = TCUConfiguration.from_dict(tcu_configuration_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


