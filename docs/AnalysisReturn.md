# AnalysisReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | A name of the contrast being performed. | [optional] [default to undefined]
**description** | **string** | A long form description of how the contrast was performed | [optional] [default to undefined]
**weights** | **Array&lt;number&gt;** | Weight applied to each condition, must be the same length as the conditions attribute. | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**study** | **string** |  | [optional] [default to undefined]
**images** | [**AnalysisReturnRelationshipsImages**](AnalysisReturnRelationshipsImages.md) |  | [optional] [default to undefined]
**points** | [**AnalysisReturnRelationshipsPoints**](AnalysisReturnRelationshipsPoints.md) |  | [optional] [default to undefined]
**conditions** | [**AnalysisReturnRelationshipsConditions**](AnalysisReturnRelationshipsConditions.md) |  | [optional] [default to undefined]
**table_id** | **string** |  | [optional] [default to undefined]
**entities** | [**Array&lt;Entity&gt;**](Entity.md) |  | [optional] [default to undefined]
**order** | **number** |  | [optional] [default to undefined]
**metadata** | **object** |  | [optional] [default to undefined]
**has_coordinates** | **boolean** |  | [optional] [default to undefined]
**has_images** | **boolean** |  | [optional] [default to undefined]
**has_z_maps** | **boolean** |  | [optional] [default to undefined]
**has_t_maps** | **boolean** |  | [optional] [default to undefined]
**has_beta_and_variance_maps** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisReturn } from './api';

const instance: AnalysisReturn = {
    name,
    description,
    weights,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    study,
    images,
    points,
    conditions,
    table_id,
    entities,
    order,
    metadata,
    has_coordinates,
    has_images,
    has_z_maps,
    has_t_maps,
    has_beta_and_variance_maps,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
