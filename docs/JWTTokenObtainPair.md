# JWTTokenObtainPair


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**otp_code** | **str** |  | [optional] 
**device_type** | **str** |  | [optional] 
**device_os** | **str** |  | [optional] 
**app_version** | **str** |  | [optional] 
**push_notification_key** | **str** |  | [optional] 
**username** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from opencarwings_client.models.jwt_token_obtain_pair import JWTTokenObtainPair

# TODO update the JSON string below
json = "{}"
# create an instance of JWTTokenObtainPair from a JSON string
jwt_token_obtain_pair_instance = JWTTokenObtainPair.from_json(json)
# print the JSON string representation of the object
print(JWTTokenObtainPair.to_json())

# convert the object into a dict
jwt_token_obtain_pair_dict = jwt_token_obtain_pair_instance.to_dict()
# create an instance of JWTTokenObtainPair from a dict
jwt_token_obtain_pair_from_dict = JWTTokenObtainPair.from_dict(jwt_token_obtain_pair_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


