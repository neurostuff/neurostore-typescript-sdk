# ReviewProgress

One reviewer\'s review of a paper, as the paper list shows it.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **string** |  | [optional] [default to undefined]
**user_name** | **string** |  | [optional] [default to undefined]
**state** | [**ReviewState**](ReviewState.md) |  | [optional] [default to undefined]
**last_seq** | **number** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**edited** | **number** | Targets the reviewer edited, added or removed. | [optional] [default to undefined]
**verified** | **number** | Targets the reviewer checked and left unchanged. | [optional] [default to undefined]
**reviewed** | **number** | Judgeable targets of the source that the reviewer verified, edited, added or removed. Unlike edited and verified, which count every provenance key, this counts only among the source\&#39;s judgeable targets. | [optional] [default to undefined]

## Example

```typescript
import { ReviewProgress } from './api';

const instance: ReviewProgress = {
    user_id,
    user_name,
    state,
    last_seq,
    updated_at,
    edited,
    verified,
    reviewed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
