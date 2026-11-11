# AnalysisQueryContrastSideOneOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**has_patients** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**has_healthy** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**medical_condition** | [**AnalysisQueryNormalized**](AnalysisQueryNormalized.md) |  | [optional] [default to undefined]
**timepoint** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**arm_kind** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**facet** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryContrastSideOneOf } from './api';

const instance: AnalysisQueryContrastSideOneOf = {
    name,
    has_patients,
    has_healthy,
    medical_condition,
    timepoint,
    arm_kind,
    facet,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
