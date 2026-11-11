# AnalysisQuery

Criteria on a pipeline analysis. Group criteria (medical_condition, species, has_patients, has_healthy) match when any group the analysis ran on matches. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**medical_condition** | [**AnalysisQueryMedicalCondition**](AnalysisQueryMedicalCondition.md) |  | [optional] [default to undefined]
**has_patients** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**has_healthy** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**species** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**task** | [**AnalysisQueryNormalized**](AnalysisQueryNormalized.md) |  | [optional] [default to undefined]
**spatial_scope** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**coordinate_space** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**measure_type** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**measure_family** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**details_type** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**is_meta_analysis** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**n** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**has_coordinates** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**role** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**contrast** | [**AnalysisQueryContrast**](AnalysisQueryContrast.md) |  | [optional] [default to undefined]
**design** | [**AnalysisQueryDesign**](AnalysisQueryDesign.md) |  | [optional] [default to undefined]
**acquisitions** | [**AnalysisQueryAcquisitions**](AnalysisQueryAcquisitions.md) |  | [optional] [default to undefined]
**coordinate_sets** | [**AnalysisQueryCoordinateSets**](AnalysisQueryCoordinateSets.md) |  | [optional] [default to undefined]
**details** | [**AnalysisQueryDetails**](AnalysisQueryDetails.md) |  | [optional] [default to undefined]
**effect** | [**AnalysisQueryEffect**](AnalysisQueryEffect.md) |  | [optional] [default to undefined]
**groups** | [**AnalysisQueryGroups**](AnalysisQueryGroups.md) |  | [optional] [default to undefined]
**inference_settings** | [**AnalysisQueryInferenceSettings**](AnalysisQueryInferenceSettings.md) |  | [optional] [default to undefined]
**model_estimation** | [**AnalysisQueryModelEstimation**](AnalysisQueryModelEstimation.md) |  | [optional] [default to undefined]
**preprocessing** | [**AnalysisQueryPreprocessing**](AnalysisQueryPreprocessing.md) |  | [optional] [default to undefined]
**regions** | [**AnalysisQueryRegions**](AnalysisQueryRegions.md) |  | [optional] [default to undefined]
**tasks** | [**AnalysisQueryTasks**](AnalysisQueryTasks.md) |  | [optional] [default to undefined]
**or** | **Array&lt;{ [key: string]: any; }&gt;** | Sub-queries, any of which may match; each takes this object\&#39;s criteria. (Not a $ref to this schema, which resolvers that inline references cannot expand.)  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQuery } from './api';

const instance: AnalysisQuery = {
    name,
    medical_condition,
    has_patients,
    has_healthy,
    species,
    task,
    spatial_scope,
    coordinate_space,
    measure_type,
    measure_family,
    details_type,
    is_meta_analysis,
    n,
    has_coordinates,
    role,
    contrast,
    design,
    acquisitions,
    coordinate_sets,
    details,
    effect,
    groups,
    inference_settings,
    model_estimation,
    preprocessing,
    regions,
    tasks,
    or,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
