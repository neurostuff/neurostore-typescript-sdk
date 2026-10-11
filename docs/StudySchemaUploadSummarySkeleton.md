# StudySchemaUploadSummarySkeleton

For a parse, what it did to the study\'s analyses.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **number** |  | [optional] [default to undefined]
**updated** | **number** |  | [optional] [default to undefined]
**superseded** | **number** | Analyses moved to the history study because this version dropped their key. | [optional] [default to undefined]
**omitted_analyses** | **number** | How many text or figure analyses the parse lists as read and left out. Their reasons are kept in the study\&#39;s metadata, not returned here.  | [optional] [default to undefined]
**aliased** | [**Array&lt;StudySchemaUploadSummarySkeletonAliasedInner&gt;**](StudySchemaUploadSummarySkeletonAliasedInner.md) | Analyses an original re-parse reads from other cells (same table and name, new key), one pair each; their entities keep the old hash as an alias.  | [optional] [default to undefined]
**alias_conflicts** | [**Array&lt;StudySchemaUploadSummarySkeletonAliasConflictsInner&gt;**](StudySchemaUploadSummarySkeletonAliasConflictsInner.md) | Re-read analyses whose new hash already belongs to another entity; nothing is re-hashed for that entity class and its claims stay where they are. Present for an original parse, absent for a revision.  | [optional] [default to undefined]
**rename_candidates** | [**Array&lt;StudySchemaRenameCandidate&gt;**](StudySchemaRenameCandidate.md) | Analyses read from the same place under a new name. Each old entity is linked to a candidate entity for the new name as renamed_by_extractor; no claims move. Present for an original parse, absent for a revision.  | [optional] [default to undefined]
**orphaned_claims** | [**Array&lt;StudySchemaUploadSummarySkeletonOrphanedClaimsInner&gt;**](StudySchemaUploadSummarySkeletonOrphanedClaimsInner.md) | Entities that hold claims and stayed on a superseded (history) analysis: not re-hashed onto a successor, not linked as a rename candidate, and not copied by a split or merge verdict. Always present; empty when none.  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummarySkeleton } from './api';

const instance: StudySchemaUploadSummarySkeleton = {
    created,
    updated,
    superseded,
    omitted_analyses,
    aliased,
    alias_conflicts,
    rename_candidates,
    orphaned_claims,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
