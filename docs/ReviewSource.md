# ReviewSource


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**base_study_id** | **string** |  | [default to undefined]
**label** | **string** |  | [default to undefined]
**origin** | **string** | pipeline_run when the source names a pipeline config and a run, else upload. | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**total** | **number** | Targets a reviewer can judge in the source\&#39;s record, its extracted values and its coordinate parse\&#39;s analyses. | [default to undefined]
**reviews** | [**Array&lt;ReviewProgress&gt;**](ReviewProgress.md) |  | [default to undefined]
**assignees** | [**Array&lt;ReviewAssignee&gt;**](ReviewAssignee.md) | The users the paper (base study) is assigned to. | [default to undefined]

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
    assignees,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
