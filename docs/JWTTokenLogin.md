# JWTTokenLogin


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**refresh** | **str** |  | 
**access** | **str** |  | [optional] [readonly] 
**user_id** | **int** |  | [optional] [readonly] 
**username** | **str** |  | [optional] 

## Example

```python
from opencarwings_client.models.jwt_token_login import JWTTokenLogin

# TODO update the JSON string below
json = "{}"
# create an instance of JWTTokenLogin from a JSON string
jwt_token_login_instance = JWTTokenLogin.from_json(json)
# print the JSON string representation of the object
print(JWTTokenLogin.to_json())

# convert the object into a dict
jwt_token_login_dict = jwt_token_login_instance.to_dict()
# create an instance of JWTTokenLogin from a dict
jwt_token_login_from_dict = JWTTokenLogin.from_dict(jwt_token_login_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


