# AnnotationPipelineExtensionPipelinesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Pipeline extractor name. | [default to undefined]
**version** | **string** | Optional pipeline version to use; latest is selected when omitted. | [optional] [default to undefined]
**config_id** | **string** | Optional specific pipeline config identifier to use. | [optional] [default to undefined]
**columns** | **Array&lt;string&gt;** | Feature columns to add to each annotation note. | [default to undefined]

## Example

```typescript
import { AnnotationPipelineExtensionPipelinesInner } from './api';

const instance: AnnotationPipelineExtensionPipelinesInner = {
    name,
    version,
    config_id,
    columns,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
