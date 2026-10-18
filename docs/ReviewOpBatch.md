# ReviewOpBatch


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expected_last_seq** | **number** | The review\&#39;s last_seq the batch was made against. | [default to undefined]
**ops** | **Array&lt;object&gt;** | The batch\&#39;s ops, at least and at most as many as the contract served at GET /api/review/schemas/review-ops allows.  | [default to undefined]

## Example

```typescript
import { ReviewOpBatch } from './api';

const instance: ReviewOpBatch = {
    expected_last_seq,
    ops,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
