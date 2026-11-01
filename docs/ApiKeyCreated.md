# ApiKeyCreated


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**prefix** | **string** | the first characters of the key, to tell keys apart | [optional] [default to undefined]
**scopes** | **Set&lt;string&gt;** | &#x60;read&#x60; allows GET requests; &#x60;write&#x60; allows every method. | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**last_used_at** | **string** |  | [optional] [default to undefined]
**revoked_at** | **string** |  | [optional] [default to undefined]
**key** | **string** | the full key; it cannot be retrieved again | [optional] [default to undefined]

## Example

```typescript
import { ApiKeyCreated } from './api';

const instance: ApiKeyCreated = {
    id,
    name,
    prefix,
    scopes,
    created_at,
    last_used_at,
    revoked_at,
    key,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
