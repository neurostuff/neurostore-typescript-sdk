# ReviewStoredOp

An applied op as the review stores it: $defs/StoredOp of the contract served at GET /api/review/schemas/review-bundle. In an op result each one also carries `inverse`, the ops that undo it without their client_op_ids, unless it is a note; the bundle\'s stored ops do not. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inverse** | **Array&lt;object&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { ReviewStoredOp } from './api';

const instance: ReviewStoredOp = {
    inverse,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
