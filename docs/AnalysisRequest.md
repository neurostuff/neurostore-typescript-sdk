# AnalysisRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | A name of the contrast being performed. | [optional] [default to undefined]
**description** | **string** | A long form description of how the contrast was performed | [optional] [default to undefined]
**weights** | **Array&lt;number&gt;** | Weight applied to each condition, must be the same length as the conditions attribute. | [optional] [default to undefined]
**study** | **string** |  | [optional] [default to undefined]
**images** | [**AnalysisRequestRelationshipsImages**](AnalysisRequestRelationshipsImages.md) |  | [optional] [default to undefined]
**points** | [**AnalysisRequestRelationshipsPoints**](AnalysisRequestRelationshipsPoints.md) |  | [optional] [default to undefined]
**conditions** | [**AnalysisRequestRelationshipsConditions**](AnalysisRequestRelationshipsConditions.md) |  | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**table_id** | **string** |  | [optional] [default to undefined]
**entities** | [**Array&lt;Entity&gt;**](Entity.md) |  | [optional] [default to undefined]
**order** | **number** |  | [optional] [default to undefined]
**metadata** | **object** |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisRequest } from './api';

const instance: AnalysisRequest = {
    name,
    description,
    weights,
    study,
    images,
    points,
    conditions,
    id,
    _public,
    table_id,
    entities,
    order,
    metadata,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
