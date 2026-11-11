# AnalysisQueryInferenceSettings

The analysis\'s inference settings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inference_level** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**height_threshold_value** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**height_threshold_type** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**cluster_extent_threshold** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**clusterwise_threshold_value** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**multiple_comparison_method** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**correction_scope** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**alpha_level** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**tfce_used** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**permutation_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryInferenceSettings } from './api';

const instance: AnalysisQueryInferenceSettings = {
    inference_level,
    height_threshold_value,
    height_threshold_type,
    cluster_extent_threshold,
    clusterwise_threshold_value,
    multiple_comparison_method,
    correction_scope,
    alpha_level,
    tfce_used,
    permutation_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
