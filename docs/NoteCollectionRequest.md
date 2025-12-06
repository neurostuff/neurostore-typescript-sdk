# NoteCollectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**note** | **object** | The note will contain all note_keys as keys and have a value of either null or the value type specified in note_keys. | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]

## Example

```typescript
import { NoteCollectionRequest } from './api';

const instance: NoteCollectionRequest = {
    note,
    id,
    _public,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
