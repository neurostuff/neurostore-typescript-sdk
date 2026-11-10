# AnalysisQueryResultResultsInnerAnalysesInnerFeatures

Only when `detail` is `features`. The analysis\'s display and every column its criteria read, named as stored (`is_meta_analysis`, `species`, `task_ids`, `medical_condition_role_ids`, `arm_kinds`, `contrast_positive_timepoints`, and the analysis\'s `role` and `has_coordinates`), with `task_family_ids` and the extraction they were read from. A column the record is silent on is absent. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config_id** | **string** | The pipeline config of the record the features were read from. | [optional] [default to undefined]
**updated_at** | **string** | When the features were last written. Every re-ingest of the paper rewrites them, changed or not.  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResultResultsInnerAnalysesInnerFeatures } from './api';

const instance: AnalysisQueryResultResultsInnerAnalysesInnerFeatures = {
    config_id,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
