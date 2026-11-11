# AnalysisFeatures

Only when `detail` is `features`: what the analysis\'s record says, in the shape of the query, each criterion\'s value under its path. A normalized criterion has its mapped `ids` (and `role_ids`, `family_ids`) and the record\'s wording as `text`; a text criterion has the record\'s wording. An item the record is silent on is absent. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**medical_condition** | [**AnalysisFeaturesMedicalCondition**](AnalysisFeaturesMedicalCondition.md) |  | [optional] [default to undefined]
**has_patients** | **boolean** |  | [optional] [default to undefined]
**has_healthy** | **boolean** |  | [optional] [default to undefined]
**species** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**task** | [**AnalysisFeaturesTask**](AnalysisFeaturesTask.md) |  | [optional] [default to undefined]
**spatial_scope** | **string** |  | [optional] [default to undefined]
**coordinate_space** | **string** |  | [optional] [default to undefined]
**measure_type** | **string** |  | [optional] [default to undefined]
**measure_family** | **string** |  | [optional] [default to undefined]
**details_type** | **string** |  | [optional] [default to undefined]
**is_meta_analysis** | **boolean** |  | [optional] [default to undefined]
**n** | **number** |  | [optional] [default to undefined]
**contrast** | [**AnalysisFeaturesContrast**](AnalysisFeaturesContrast.md) |  | [optional] [default to undefined]
**design** | [**AnalysisFeaturesDesign**](AnalysisFeaturesDesign.md) |  | [optional] [default to undefined]
**groups** | [**AnalysisFeaturesGroups**](AnalysisFeaturesGroups.md) |  | [optional] [default to undefined]
**inference_settings** | [**AnalysisFeaturesInferenceSettings**](AnalysisFeaturesInferenceSettings.md) |  | [optional] [default to undefined]
**acquisitions** | [**AnalysisFeaturesAcquisitions**](AnalysisFeaturesAcquisitions.md) |  | [optional] [default to undefined]
**preprocessing** | [**AnalysisFeaturesPreprocessing**](AnalysisFeaturesPreprocessing.md) |  | [optional] [default to undefined]
**model_estimation** | [**AnalysisFeaturesModelEstimation**](AnalysisFeaturesModelEstimation.md) |  | [optional] [default to undefined]
**effect** | [**AnalysisFeaturesEffect**](AnalysisFeaturesEffect.md) |  | [optional] [default to undefined]
**details** | [**AnalysisFeaturesDetails**](AnalysisFeaturesDetails.md) |  | [optional] [default to undefined]
**regions** | [**AnalysisFeaturesRegions**](AnalysisFeaturesRegions.md) |  | [optional] [default to undefined]
**coordinate_sets** | [**AnalysisFeaturesCoordinateSets**](AnalysisFeaturesCoordinateSets.md) |  | [optional] [default to undefined]
**tasks** | [**AnalysisFeaturesTasks**](AnalysisFeaturesTasks.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisFeatures } from './api';

const instance: AnalysisFeatures = {
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
    contrast,
    design,
    groups,
    inference_settings,
    acquisitions,
    preprocessing,
    model_estimation,
    effect,
    details,
    regions,
    coordinate_sets,
    tasks,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
