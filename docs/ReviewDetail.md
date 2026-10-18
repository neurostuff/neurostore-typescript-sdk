# ReviewDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**source_id** | **string** |  | [default to undefined]
**user_id** | **string** |  | [default to undefined]
**state** | [**ReviewState**](ReviewState.md) |  | [default to undefined]
**set_aside** | [**ReviewSetAside**](ReviewSetAside.md) |  | [optional] [default to undefined]
**last_seq** | **number** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**updated_at** | **string** |  | [default to undefined]
**record** | **object** | The extraction record with the review\&#39;s ops applied. | [optional] [default to undefined]
**coordinate_revision** | **object** |  | [optional] [default to undefined]
**provenance** | **object** |  | [optional] [default to undefined]
**annotations** | **object** |  | [optional] [default to undefined]
**ops** | [**Array&lt;ReviewStoredOp&gt;**](ReviewStoredOp.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ReviewDetail } from './api';

const instance: ReviewDetail = {
    id,
    source_id,
    user_id,
    state,
    set_aside,
    last_seq,
    created_at,
    updated_at,
    record,
    coordinate_revision,
    provenance,
    annotations,
    ops,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
