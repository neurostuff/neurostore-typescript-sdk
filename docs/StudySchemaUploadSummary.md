# StudySchemaUploadSummary

What one upload changed. Keys appear for the parts uploaded.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | **string** |  | [optional] [default to undefined]
**base_study_id** | **string** |  | [optional] [default to undefined]
**study_id** | **string** | The paper\&#39;s pipeline-owned study. | [optional] [default to undefined]
**parse_id** | **string** |  | [optional] [default to undefined]
**skeleton** | [**StudySchemaUploadSummarySkeleton**](StudySchemaUploadSummarySkeleton.md) |  | [optional] [default to undefined]
**carried** | [**StudySchemaCarried**](StudySchemaCarried.md) |  | [optional] [default to undefined]
**set_aside_resolved** | [**Array&lt;StudySchemaUploadSummarySetAsideResolvedInner&gt;**](StudySchemaUploadSummarySetAsideResolvedInner.md) | For a parse: stored records whose set-aside keys (no earlier parse held them) this parse holds, re-ingested onto the new entities.  | [optional] [default to undefined]
**record** | [**StudySchemaUploadSummaryRecord**](StudySchemaUploadSummaryRecord.md) |  | [optional] [default to undefined]
**provenance** | [**{ [key: string]: PipelineRunProvenance; }**](PipelineRunProvenance.md) | The stored run behind each part of the upload, keyed parse and record. | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummary } from './api';

const instance: StudySchemaUploadSummary = {
    kind,
    base_study_id,
    study_id,
    parse_id,
    skeleton,
    carried,
    set_aside_resolved,
    record,
    provenance,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
