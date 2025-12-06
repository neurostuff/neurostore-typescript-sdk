# AnnotationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Descriptive name for the annotation. | [optional] [default to undefined]
**description** | **string** | Long form description of the annotation. | [optional] [default to undefined]
**metadata** | **object** |  | [optional] [readonly] [default to undefined]
**note_keys** | **object** | The keys (columns) in the annotation and the key\&#39;s respective data type (such as an integer or string). | [optional] [default to undefined]
**pipelines** | [**Array&lt;AnnotationPipelineExtensionPipelinesInner&gt;**](AnnotationPipelineExtensionPipelinesInner.md) | Optional pipeline descriptors used to populate annotation notes with feature columns. Each entry should include the pipeline name and the list of columns to import, along with optional version and config id.  | [optional] [default to undefined]
**notes** | [**AnnotationRequestRelationshipsNotes**](AnnotationRequestRelationshipsNotes.md) |  | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**studyset** | **string** |  | [optional] [default to undefined]
**annotation_csv** | **string** | annotation object expressed as a CSV | [default to undefined]

## Example

```typescript
import { AnnotationRequest } from './api';

const instance: AnnotationRequest = {
    name,
    description,
    metadata,
    note_keys,
    pipelines,
    notes,
    id,
    _public,
    studyset,
    annotation_csv,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
