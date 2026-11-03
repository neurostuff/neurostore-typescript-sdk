# DataSourceReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **string** | A short stable key, e.g. &#x60;ukb&#x60;. | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**kinds** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**modalities** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**part_of** | **string** | The data source (repository or consortium) this one is hosted by or part of. | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**url_kind** | **string** | Where the url came from or what it points to, e.g. &#x60;rrid&#x60;, &#x60;re3data&#x60;, &#x60;jpnd&#x60;, &#x60;checked:official&#x60;, &#x60;checked:registry&#x60;, &#x60;checked:publication&#x60;. | [optional] [default to undefined]
**rrids** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**re3data_ids** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**listed_in** | **Array&lt;string&gt;** | The catalogues the data source was found in. | [optional] [default to undefined]
**aliases** | [**Array&lt;DataSourceAlias&gt;**](DataSourceAlias.md) |  | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]

## Example

```typescript
import { DataSourceReturn } from './api';

const instance: DataSourceReturn = {
    slug,
    name,
    description,
    kinds,
    modalities,
    part_of,
    url,
    url_kind,
    rrids,
    re3data_ids,
    listed_in,
    aliases,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
