# DataSourceReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The data source\&#39;s key, e.g. &#x60;ukb&#x60;, given when it is created and never changed, so records made outside neurostore can name it before it is uploaded. | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**kinds** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**modalities** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**part_of** | **string** | The data source (repository or consortium) this one is hosted by or part of. | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**url_kind** | **string** | Where the url came from or what it points to, e.g. &#x60;rrid&#x60;, &#x60;re3data&#x60;, &#x60;jpnd&#x60;, &#x60;checked:official&#x60;, &#x60;checked:registry&#x60;, &#x60;checked:publication&#x60;. | [optional] [default to undefined]
**rrids** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**re3data_ids** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**user** | **string** | The owner\&#39;s Auth0 id, served only to the owner; null for anyone else, who sees &#x60;username&#x60;. | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]

## Example

```typescript
import { DataSourceReturn } from './api';

const instance: DataSourceReturn = {
    id,
    name,
    description,
    kinds,
    modalities,
    part_of,
    url,
    url_kind,
    rrids,
    re3data_ids,
    created_at,
    updated_at,
    user,
    username,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
