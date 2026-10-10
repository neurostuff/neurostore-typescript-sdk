# StudySchemaUploadSummaryRecordAnalyses


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**resolved** | **number** |  | [optional] [default to undefined]
**unresolved** | **Array&lt;string&gt;** | Keys (or local_ids) that resolve to no analysis; stored as FAILURE rows. | [optional] [default to undefined]
**parked** | [**Array&lt;StudySchemaSetAside&gt;**](StudySchemaSetAside.md) | Set-aside positional keys, held until a record names them by content. | [optional] [default to undefined]
**superseded** | [**Array&lt;StudySchemaUploadSummaryRecordAnalysesSupersededInner&gt;**](StudySchemaUploadSummaryRecordAnalysesSupersededInner.md) | Keys that resolve to history because a revision since split, merged or dropped them. | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummaryRecordAnalyses } from './api';

const instance: StudySchemaUploadSummaryRecordAnalyses = {
    resolved,
    unresolved,
    parked,
    superseded,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
