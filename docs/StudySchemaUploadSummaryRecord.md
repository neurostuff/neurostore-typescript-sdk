# StudySchemaUploadSummaryRecord

For a record, how its analyses and claims resolved.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config_id** | **string** |  | [optional] [default to undefined]
**analyses** | [**StudySchemaUploadSummaryRecordAnalyses**](StudySchemaUploadSummaryRecordAnalyses.md) |  | [optional] [default to undefined]
**condition_conflicts** | [**Array&lt;StudySchemaUploadSummaryRecordConditionConflictsInner&gt;**](StudySchemaUploadSummaryRecordConditionConflictsInner.md) | Record analyses whose effect cells set no conditions (the analysis gets none) because the cells contradict each other. One entry per record entry, keyed by its key, or its local_id when it has none.  | [optional] [default to undefined]
**claims** | [**StudySchemaUploadSummaryRecordClaims**](StudySchemaUploadSummaryRecordClaims.md) |  | [optional] [default to undefined]
**carried** | [**StudySchemaCarried**](StudySchemaCarried.md) |  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummaryRecord } from './api';

const instance: StudySchemaUploadSummaryRecord = {
    config_id,
    analyses,
    condition_conflicts,
    claims,
    carried,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
