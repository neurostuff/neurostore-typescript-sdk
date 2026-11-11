# AnalysisQueryGroups

The groups the analysis ran on; a number with an item per group (an age) matches when any group\'s does. Ages are in years; counts are summed over the groups; the female share is of those whose sex (or, where only that is reported, gender) is counted.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**age_mean** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_standard_deviation** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_minimum** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_maximum** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**age_median** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**female_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**male_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**female_percent** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**handedness** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**enrolled_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**acquired_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**excluded_count** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**diagnostic_instrument** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**diagnostic_system** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**clinical_characteristics** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**education_summary** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryGroups } from './api';

const instance: AnalysisQueryGroups = {
    age_mean,
    age_standard_deviation,
    age_minimum,
    age_maximum,
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
    education_summary,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
