# TableReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**t_id** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**footer** | **string** |  | [optional] [default to undefined]
**caption** | **string** |  | [optional] [default to undefined]
**study** | **string** |  | [optional] [default to undefined]
**analyses** | [**StudyReturnRelationshipsAnalyses**](StudyReturnRelationshipsAnalyses.md) |  | [optional] [default to undefined]

## Example

```typescript
import { TableReturn } from './api';

const instance: TableReturn = {
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    t_id,
    name,
    footer,
    caption,
    study,
    analyses,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
