# PipelineRunProvenance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**result_id** | **string** | The pipeline-study-result that stores the document. | [optional] [default to undefined]
**config_id** | **string** |  | [optional] [default to undefined]
**pipeline** | **string** |  | [optional] [default to undefined]
**version** | **string** |  | [optional] [default to undefined]
**commit** | **string** |  | [optional] [default to undefined]
**schema** | [**PipelineRunProvenanceSchema**](PipelineRunProvenanceSchema.md) |  | [optional] [default to undefined]
**parse_version** | **{ [key: string]: any; }** | The parse\&#39;s producer (name, version, stage, model, prompt_version). | [optional] [default to undefined]
**date_executed** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PipelineRunProvenance } from './api';

const instance: PipelineRunProvenance = {
    result_id,
    config_id,
    pipeline,
    version,
    commit,
    schema,
    parse_version,
    date_executed,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
