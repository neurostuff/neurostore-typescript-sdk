# NoteCollectionReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**note** | **object** | The note will contain all note_keys as keys and have a value of either null or the value type specified in note_keys. | [optional] [default to undefined]
**analysis** | **string** |  | [optional] [readonly] [default to undefined]
**analysis_name** | **string** |  | [optional] [readonly] [default to undefined]
**study** | **string** |  | [optional] [readonly] [default to undefined]
**study_name** | **string** |  | [optional] [readonly] [default to undefined]
**annotation** | **string** |  | [optional] [readonly] [default to undefined]
**study_year** | **number** |  | [optional] [readonly] [default to undefined]
**publication** | **string** |  | [optional] [readonly] [default to undefined]
**authors** | **string** |  | [optional] [readonly] [default to undefined]
**id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { NoteCollectionReturn } from './api';

const instance: NoteCollectionReturn = {
    note,
    analysis,
    analysis_name,
    study,
    study_name,
    annotation,
    study_year,
    publication,
    authors,
    id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
