# AnalysisQueryModelEstimation

The analysis\'s model estimation and the models it takes inputs from.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**model_family** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**model_type** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**software** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**hrf_model** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**estimator** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**terms** | [**AnalysisQueryModelEstimationTerms**](AnalysisQueryModelEstimationTerms.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryModelEstimation } from './api';

const instance: AnalysisQueryModelEstimation = {
    model_family,
    model_type,
    software,
    hrf_model,
    estimator,
    terms,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
