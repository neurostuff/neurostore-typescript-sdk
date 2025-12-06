# PipelineEmbedding


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**config_id** | **string** |  | [default to undefined]
**base_study_id** | **string** |  | [optional] [default to undefined]
**date_executed** | **string** |  | [optional] [default to undefined]
**file_inputs** | **object** |  | [optional] [default to undefined]
**status** | **string** | Current status of the pipeline execution (e.g. SUCCESS, FAILURE, ERROR, UNKNOWN) | [default to undefined]
**embedding** | **Array&lt;number&gt;** |  | [default to undefined]

## Example

```typescript
import { PipelineEmbedding } from './api';

const instance: PipelineEmbedding = {
    created_at,
    updated_at,
    config_id,
    base_study_id,
    date_executed,
    file_inputs,
    status,
    embedding,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
