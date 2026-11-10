# AnalysisQuerySample

The groups the analysis ran on; a criterion on an item of each group (an age) matches when any group\'s does. Ages are in years; counts are summed over the groups. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**age_mean** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_sd** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_min** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_max** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_median** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**female_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**male_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**female_percent** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**handedness** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**enrolled_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**acquired_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**excluded_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**diagnostic_instrument** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**diagnostic_system** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**clinical_characteristics** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**education** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQuerySample } from './api';

const instance: AnalysisQuerySample = {
    age_mean,
    age_sd,
    age_min,
    age_max,
    age_median,
    female_count,
    male_count,
    female_percent,
    handedness,
    enrolled_count,
    acquired_count,
    excluded_count,
    diagnostic_instrument,
    diagnostic_system,
    clinical_characteristics,
    education,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
