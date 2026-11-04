# StudySchemaUploadPipeline

The pipeline run that produced the record.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Default pondie. | [optional] [default to undefined]
**version** | **string** | Default the record\&#39;s extraction_metadata.extractor_version. | [optional] [default to undefined]
**commit** | **string** | The commit of the code that produced the record. Two commits of one version are different configs. | [optional] [default to undefined]
**runs** | [**Array&lt;StudySchemaRun&gt;**](StudySchemaRun.md) | The runs that made the record: its record run, and the evidence and normalize runs that filled it in, at most one per stage. The record\&#39;s config holds them in stage order with every field present, so uploads made by the same runs share one config, and a run of another model, adapter, prompt or fit gets another. A rerun with the same model and inputs is the same run and joins its config. Without runs the config is keyed as before. Validated by the service (422 SCHEMA, DUPLICATE_STAGE, DUPLICATE_RUN_ID, RUN_CONFLICT).  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadPipeline } from './api';

const instance: StudySchemaUploadPipeline = {
    name,
    version,
    commit,
    runs,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
