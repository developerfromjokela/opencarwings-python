# AccountDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_2fa_enabled** | **bool** |  | [optional] [readonly] 
**is_command_pin_set** | **bool** |  | [optional] [readonly] 
**timezone** | **str** |  | [optional] 
**email_notifications** | **bool** |  | [optional] 
**username** | **str** | Required. 16 characters or fewer. Letters, digits and /./-/_ only. | 
**email** | **str** |  | [optional] 
**units_imperial** | **bool** |  | [optional] 
**last_login** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.account_detail import AccountDetail

# TODO update the JSON string below
json = "{}"
# create an instance of AccountDetail from a JSON string
account_detail_instance = AccountDetail.from_json(json)
# print the JSON string representation of the object
print(AccountDetail.to_json())

# convert the object into a dict
account_detail_dict = account_detail_instance.to_dict()
# create an instance of AccountDetail from a dict
account_detail_from_dict = AccountDetail.from_dict(account_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


