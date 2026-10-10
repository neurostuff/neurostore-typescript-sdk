# StudySchemaUploadPipeline

The pipeline run that produced the record.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Default pondie. | [optional] [default to undefined]
**version** | **string** | Default the record\&#39;s extraction_metadata.extractor_version. | [optional] [default to undefined]
**commit** | **string** | The commit of the code that produced the record. Two commits of one version are different configs. | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadPipeline } from './api';

const instance: StudySchemaUploadPipeline = {
    name,
    version,
    commit,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
