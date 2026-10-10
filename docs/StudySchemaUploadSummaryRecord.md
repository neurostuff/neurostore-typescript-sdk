# StudySchemaUploadSummaryRecord

For a record, how its analyses and claims resolved.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config_id** | **string** |  | [optional] [default to undefined]
**analyses** | [**StudySchemaUploadSummaryRecordAnalyses**](StudySchemaUploadSummaryRecordAnalyses.md) |  | [optional] [default to undefined]
**claims** | [**StudySchemaUploadSummaryRecordClaims**](StudySchemaUploadSummaryRecordClaims.md) |  | [optional] [default to undefined]
**carried** | [**StudySchemaCarried**](StudySchemaCarried.md) |  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummaryRecord } from './api';

const instance: StudySchemaUploadSummaryRecord = {
    config_id,
    analyses,
    claims,
    carried,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
