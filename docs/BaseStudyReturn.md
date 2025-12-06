# BaseStudyReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | **object** |  | [optional] [default to undefined]
**versions** | [**Array&lt;BaseStudyVersionsInner&gt;**](BaseStudyVersionsInner.md) |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**publication** | **string** |  | [optional] [default to undefined]
**doi** | **string** |  | [optional] [default to undefined]
**pmid** | **string** |  | [optional] [default to undefined]
**authors** | **string** |  | [optional] [default to undefined]
**year** | **number** |  | [optional] [default to undefined]
**level** | **string** |  | [optional] [default to undefined]
**is_oa** | **boolean** |  | [optional] [default to undefined]
**pmcid** | **string** |  | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**features** | **object** |  | [optional] [default to undefined]

## Example

```typescript
import { BaseStudyReturn } from './api';

const instance: BaseStudyReturn = {
    metadata,
    versions,
    name,
    description,
    publication,
    doi,
    pmid,
    authors,
    year,
    level,
    is_oa,
    pmcid,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    features,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
