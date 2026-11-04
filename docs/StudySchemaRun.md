# StudySchemaRun

One run behind a record, as the pipeline\'s runs table first stored it. A run is one combination of model and inputs; reruns of it carry the same run_id and fields. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**run_id** | **string** | Required. Names one run; a run_id stored with other fields is refused (RUN_CONFLICT). | [optional] [default to undefined]
**kind** | **string** | model (a model made the output) or migration (an older output carried over). | [optional] [default to undefined]
**stage** | **string** | Required. record, evidence or normalize. | [optional] [default to undefined]
**source** | **string** | Required. The record source the run made or read. | [optional] [default to undefined]
**pipeline** | **string** | The pipeline that ran the stage. | [optional] [default to undefined]
**version** | **string** | The pipeline\&#39;s version. | [optional] [default to undefined]
**model** | **string** |  | [optional] [default to undefined]
**adapter** | **string** | repo@revision of the adapter the model ran with. | [optional] [default to undefined]
**prompt_version** | **string** |  | [optional] [default to undefined]
**schema_version** | **string** |  | [optional] [default to undefined]
**code_commit** | **string** |  | [optional] [default to undefined]
**machine** | **string** |  | [optional] [default to undefined]
**fit** | **string** | For a normalize run, the fingerprint of the fitted normalization model (the task and contrast clustering) it assigned with. A refit is a new run.  | [optional] [default to undefined]
**created_at** | **string** | Required. When the run was made, ISO 8601. | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaRun } from './api';

const instance: StudySchemaRun = {
    run_id,
    kind,
    stage,
    source,
    pipeline,
    version,
    model,
    adapter,
    prompt_version,
    schema_version,
    code_commit,
    machine,
    fit,
    created_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
