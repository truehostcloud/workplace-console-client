# TokenRefresh


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**refresh** | **str** |  | 
**access** | **str** |  | [optional] [readonly] 

## Example

```python
from workplace_console_client.models.token_refresh import TokenRefresh

# TODO update the JSON string below
json = "{}"
# create an instance of TokenRefresh from a JSON string
token_refresh_instance = TokenRefresh.from_json(json)
# print the JSON string representation of the object
print(TokenRefresh.to_json())

# convert the object into a dict
token_refresh_dict = token_refresh_instance.to_dict()
# create an instance of TokenRefresh from a dict
token_refresh_from_dict = TokenRefresh.from_dict(token_refresh_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


