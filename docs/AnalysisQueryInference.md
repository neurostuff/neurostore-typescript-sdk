# AnalysisQueryInference

The analysis\'s inference settings. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**level** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**height_threshold** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**height_threshold_type** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**cluster_extent** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**cluster_threshold** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**correction** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**correction_scope** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**alpha** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**tfce** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**permutations** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryInference } from './api';

const instance: AnalysisQueryInference = {
    level,
    height_threshold,
    height_threshold_type,
    cluster_extent,
    cluster_threshold,
    correction,
    correction_scope,
    alpha,
    tfce,
    permutations,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
