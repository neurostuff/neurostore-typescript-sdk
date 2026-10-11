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
**role** | **string** | What the coordinates are for (study_schema CoordinateRole): &#x60;result&#x60;, &#x60;anchor&#x60;, &#x60;localization&#x60;, &#x60;reference&#x60; or &#x60;other&#x60;; an open vocabulary, so the source\&#39;s own wording may appear. Only a result is released in a studyset. Null on an analysis from before roles, which is read as a result, except on a set the study_schema ingester wrote, which is unclassified. | [optional] [default to undefined]
**relabelled_by** | **string** | The parse_id of the reviewed revision whose relabel verdict set &#x60;role&#x60;; a later parse does not replace a relabelled role. Null while the role is the classifier\&#39;s, whose name and version are in &#x60;metadata.role_source&#x60; (study_schema\&#39;s &#x60;role_source&#x60;). | [optional] [default to undefined]
**outcome** | **string** | Whether anything survived the analysis\&#39;s threshold (study_schema AnalysisOutcome), from the extraction record. The ingester sets it only on results. | [optional] [default to undefined]
**from_prior_study** | **boolean** | The coordinates are quoted from an earlier study, not this one\&#39;s. | [optional] [default to undefined]
**source_id** | **string** | ID of the analysis this one was cloned from, if any. | [optional] [readonly] [default to undefined]
**point_count** | **number** | Number of point coordinates linked to this analysis. | [optional] [default to undefined]
**image_count** | **number** | Number of images linked to this analysis. | [optional] [default to undefined]
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
    role,
    relabelled_by,
    outcome,
    from_prior_study,
    source_id,
    point_count,
    image_count,
    has_coordinates,
    has_images,
    has_z_maps,
    has_t_maps,
    has_beta_and_variance_maps,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
