# AnalysisQueryResultResultsInnerAnalysesInnerFeatures

Only when `detail` is `features`. The analysis\'s display and the `analysis_features` columns its criteria read, named as stored (`is_meta_analysis`, `species`, `task_ids`, `task_family_ids`, `arm_kinds`, `contrast_positive_timepoints`), with the extraction they were read from. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config_id** | **string** | The pipeline config of the record the features were read from. | [optional] [default to undefined]
**updated_at** | **string** | When the features were last written; a re-ingest that changes them moves it.  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResultResultsInnerAnalysesInnerFeatures } from './api';

const instance: AnalysisQueryResultResultsInnerAnalysesInnerFeatures = {
    config_id,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
