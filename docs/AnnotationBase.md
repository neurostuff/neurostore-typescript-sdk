# AnnotationBase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Descriptive name for the annotation. | [optional] [default to undefined]
**description** | **string** | Long form description of the annotation. | [optional] [default to undefined]
**metadata** | **object** | object describing metadata about the annotation, such as software used or descriptions of the keys used in the annotation. | [optional] [default to undefined]
**note_keys** | **object** | The keys (columns) in the annotation and the key\&#39;s respective data type (such as an integer or string). | [optional] [default to undefined]

## Example

```typescript
import { AnnotationBase } from './api';

const instance: AnnotationBase = {
    name,
    description,
    metadata,
    note_keys,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
