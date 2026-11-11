# AnalysisQueryPreprocessing

The preprocessing of the analysis\'s model and of the models it takes inputs from.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**smoothing_fwhm_mm** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**software** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**steps** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryPreprocessing } from './api';

const instance: AnalysisQueryPreprocessing = {
    smoothing_fwhm_mm,
    software,
    steps,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
