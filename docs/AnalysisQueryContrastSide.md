# AnalysisQueryContrastSide

Criteria on one side of the contrast: what the cells signed onto it carry, through their factor levels. `name` is the side\'s text (its cells\' labels or levels and their conditions\' names); has_patients, has_healthy and medical_condition read the side\'s groups as the top-level criteria read the analysis\'s; `timepoint` is a timepoint\'s relation_to_intervention, `arm_kind` an arm\'s kind, and `facet` one of the side\'s contrast-key facets (`valence:negative`, `~wording`, a baseline kind such as `fixation`). A text criterion in its place is shorthand for its `name`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**any** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**all** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**none** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**when_silent** | [**AnalysisQueryWhenSilent**](AnalysisQueryWhenSilent.md) |  | [optional] [default to undefined]
**name** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**has_patients** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**has_healthy** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**medical_condition** | [**AnalysisQueryNormalized**](AnalysisQueryNormalized.md) |  | [optional] [default to undefined]
**timepoint** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**arm_kind** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**facet** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryContrastSide } from './api';

const instance: AnalysisQueryContrastSide = {
    any,
    all,
    none,
    when_silent,
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
