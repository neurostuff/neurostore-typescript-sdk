# AnalysisQuery

Criteria on a pipeline analysis. Group criteria (medical_condition, species, has_patients, has_healthy) match when any group the analysis ran on matches. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**medical_condition** | [**AnalysisQueryMedicalCondition**](AnalysisQueryMedicalCondition.md) |  | [optional] [default to undefined]
**has_patients** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**has_healthy** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**species** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**task** | [**AnalysisQueryNormalized**](AnalysisQueryNormalized.md) |  | [optional] [default to undefined]
**spatial_scope** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**coordinate_space** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**measure_type** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**measure_family** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**details_type** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**is_meta_analysis** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**n** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**has_coordinates** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**role** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**contrast** | [**AnalysisQueryContrast**](AnalysisQueryContrast.md) |  | [optional] [default to undefined]
**design** | [**AnalysisQueryDesign**](AnalysisQueryDesign.md) |  | [optional] [default to undefined]
**sample** | [**AnalysisQuerySample**](AnalysisQuerySample.md) |  | [optional] [default to undefined]
**inference** | [**AnalysisQueryInference**](AnalysisQueryInference.md) |  | [optional] [default to undefined]
**acquisition** | [**AnalysisQueryAcquisition**](AnalysisQueryAcquisition.md) |  | [optional] [default to undefined]
**preprocessing** | [**AnalysisQueryPreprocessing**](AnalysisQueryPreprocessing.md) |  | [optional] [default to undefined]
**model** | [**AnalysisQueryModel**](AnalysisQueryModel.md) |  | [optional] [default to undefined]
**statistic** | [**AnalysisQueryStatistic**](AnalysisQueryStatistic.md) |  | [optional] [default to undefined]
**connectivity** | [**AnalysisQueryConnectivity**](AnalysisQueryConnectivity.md) |  | [optional] [default to undefined]
**region** | [**AnalysisQueryRegion**](AnalysisQueryRegion.md) |  | [optional] [default to undefined]
**coordinates** | [**AnalysisQueryCoordinates**](AnalysisQueryCoordinates.md) |  | [optional] [default to undefined]
**task_details** | [**AnalysisQueryTaskDetails**](AnalysisQueryTaskDetails.md) |  | [optional] [default to undefined]
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
    sample,
    inference,
    acquisition,
    preprocessing,
    model,
    statistic,
    connectivity,
    region,
    coordinates,
    task_details,
    or,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
