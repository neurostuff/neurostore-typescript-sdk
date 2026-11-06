# AnalysisQuery

Criteria on a pipeline analysis. Group criteria (diagnosis, species, has_patients, has_healthy) match when any group the analysis ran on matches. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**diagnosis** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**has_patients** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**has_healthy** | [**AnalysisQueryBoolean**](AnalysisQueryBoolean.md) |  | [optional] [default to undefined]
**species** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**task** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
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
**or** | **Array&lt;{ [key: string]: any; }&gt;** | Sub-queries, any of which may match; each takes this object\&#39;s criteria. (Not a $ref to this schema, which resolvers that inline references cannot expand.)  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQuery } from './api';

const instance: AnalysisQuery = {
    diagnosis,
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
    or,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
