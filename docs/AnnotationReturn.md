# AnnotationReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Descriptive name for the annotation. | [optional] [default to undefined]
**description** | **string** | Long form description of the annotation. | [optional] [default to undefined]
**metadata** | **object** |  | [optional] [readonly] [default to undefined]
**note_keys** | **object** | The keys (columns) in the annotation and the key\&#39;s respective data type (such as an integer or string). | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**source** | **string** |  | [optional] [default to undefined]
**source_id** | **string** |  | [optional] [default to undefined]
**source_updated_at** | **string** |  | [optional] [readonly] [default to undefined]
**notes** | [**AnnotationReturnRelationshipsNotes**](AnnotationReturnRelationshipsNotes.md) |  | [optional] [default to undefined]
**studyset** | **string** |  | [optional] [default to undefined]
**annotation_csv** | **string** | annotation object expressed as a CSV | [default to undefined]

## Example

```typescript
import { AnnotationReturn } from './api';

const instance: AnnotationReturn = {
    name,
    description,
    metadata,
    note_keys,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    source,
    source_id,
    source_updated_at,
    notes,
    studyset,
    annotation_csv,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
