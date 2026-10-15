# ReviewSource


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**base_study_id** | **string** |  | [optional] [default to undefined]
**label** | **string** |  | [optional] [default to undefined]
**origin** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**total** | **number** | Targets a reviewer can judge in the source\&#39;s record, its extracted values and its coordinate parse\&#39;s analyses. | [optional] [default to undefined]
**reviews** | [**Array&lt;ReviewProgress&gt;**](ReviewProgress.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ReviewSource } from './api';

const instance: ReviewSource = {
    id,
    base_study_id,
    label,
    origin,
    created_at,
    total,
    reviews,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
