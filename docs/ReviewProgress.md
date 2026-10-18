# ReviewProgress

One reviewer\'s review of a paper, as the paper list shows it.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **string** |  | [default to undefined]
**user_name** | **string** |  | [default to undefined]
**state** | [**ReviewState**](ReviewState.md) |  | [default to undefined]
**set_aside** | [**ReviewSetAside**](ReviewSetAside.md) |  | [optional] [default to undefined]
**last_seq** | **number** |  | [default to undefined]
**updated_at** | **string** |  | [default to undefined]
**edited** | **number** | Targets the reviewer edited, added or removed. | [default to undefined]
**verified** | **number** | Targets the reviewer checked and left unchanged. | [default to undefined]
**reviewed** | **number** | Judgeable targets of the source that the reviewer verified, edited, added or removed. Unlike edited and verified, which count every provenance key, this counts only among the source\&#39;s judgeable targets. | [default to undefined]
**op_count** | **number** | The ops the reviewer has applied to this review. | [default to undefined]
**last_edit_at** | **string** | When the reviewer last applied an op; null before any. | [default to undefined]

## Example

```typescript
import { ReviewProgress } from './api';

const instance: ReviewProgress = {
    user_id,
    user_name,
    state,
    set_aside,
    last_seq,
    updated_at,
    edited,
    verified,
    reviewed,
    op_count,
    last_edit_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
