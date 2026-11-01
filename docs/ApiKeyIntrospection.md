# ApiKeyIntrospection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | **string** | the owner\&#39;s external id | [optional] [default to undefined]
**name** | **string** | the owner\&#39;s display name | [optional] [default to undefined]
**scopes** | **Set&lt;string&gt;** | &#x60;read&#x60; allows GET requests; &#x60;write&#x60; allows every method. | [optional] [default to undefined]

## Example

```typescript
import { ApiKeyIntrospection } from './api';

const instance: ApiKeyIntrospection = {
    user,
    name,
    scopes,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
