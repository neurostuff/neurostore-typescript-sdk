# UserResourceAttributes

common resource attributes

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | **string** | The owner\&#39;s Auth0 id, served only to the owner; null for anyone else, who sees &#x60;username&#x60;. | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]

## Example

```typescript
import { UserResourceAttributes } from './api';

const instance: UserResourceAttributes = {
    user,
    username,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
