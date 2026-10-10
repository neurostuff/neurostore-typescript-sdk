# StudySchemaUploadSummarySkeleton

For a parse, what it did to the study\'s analyses.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **number** |  | [optional] [default to undefined]
**updated** | **number** |  | [optional] [default to undefined]
**superseded** | **number** | Analyses moved to the history study because this version dropped their key. | [optional] [default to undefined]
**not_uploaded** | **Array&lt;string&gt;** | Keys of analyses whose role is not uploaded. | [optional] [default to undefined]
**aliased** | [**Array&lt;StudySchemaUploadSummarySkeletonAliasedInner&gt;**](StudySchemaUploadSummarySkeletonAliasedInner.md) | Analyses an original re-parse reads from other cells (same table and name, new key), one pair each; their entities keep the old hash as an alias.  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummarySkeleton } from './api';

const instance: StudySchemaUploadSummarySkeleton = {
    created,
    updated,
    superseded,
    not_uploaded,
    aliased,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
