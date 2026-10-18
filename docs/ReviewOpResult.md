# ReviewOpResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ops** | [**Array&lt;ReviewStoredOp&gt;**](ReviewStoredOp.md) |  | [default to undefined]
**last_seq** | **number** |  | [default to undefined]
**record** | **object** |  | [default to undefined]
**coordinate_revision** | **object** |  | [default to undefined]
**provenance** | **object** |  | [default to undefined]
**annotations** | **object** |  | [default to undefined]
**hidden** | **object** | The hidden set of the new record, as in the bundle. | [default to undefined]
**entities** | **Array&lt;object&gt;** | The entity index of the new record, as in the bundle. | [optional] [default to undefined]

## Example

```typescript
import { ReviewOpResult } from './api';

const instance: ReviewOpResult = {
    ops,
    last_seq,
    record,
    coordinate_revision,
    provenance,
    annotations,
    hidden,
    entities,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
