# StudySchemaUploadSummarySkeleton

For a parse, what it did to the study\'s analyses.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **number** |  | [optional] [default to undefined]
**updated** | **number** |  | [optional] [default to undefined]
**superseded** | **number** | Analyses moved to the history study because this version dropped their key. | [optional] [default to undefined]
**omitted_analyses** | **number** | How many text or figure analyses the parse lists as read and left out. Their reasons are kept in the study\&#39;s metadata, not returned here.  | [optional] [default to undefined]
**orphaned_claims** | [**Array&lt;StudySchemaUploadSummarySkeletonOrphanedClaimsInner&gt;**](StudySchemaUploadSummarySkeletonOrphanedClaimsInner.md) | Entities that hold claims and stayed on a superseded (history) analysis, not copied by a split or merge verdict. A changed name or point gives a new key, so the new analysis starts with no claims and the old one\&#39;s are reported here. Always present; empty when none.  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummarySkeleton } from './api';

const instance: StudySchemaUploadSummarySkeleton = {
    created,
    updated,
    superseded,
    omitted_analyses,
    orphaned_claims,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
