# AnnotationPipelineExtension


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pipelines** | [**Array&lt;AnnotationPipelineExtensionPipelinesInner&gt;**](AnnotationPipelineExtensionPipelinesInner.md) | Optional pipeline descriptors used to populate annotation notes with feature columns. Each entry should include the pipeline name and the list of columns to import, along with optional version and config id.  | [optional] [default to undefined]

## Example

```typescript
import { AnnotationPipelineExtension } from './api';

const instance: AnnotationPipelineExtension = {
    pipelines,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
