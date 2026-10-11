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
**role** | **string** | What the coordinates are for (study_schema CoordinateRole): &#x60;result&#x60;, &#x60;anchor&#x60;, &#x60;localization&#x60;, &#x60;reference&#x60; or &#x60;other&#x60;; an open vocabulary, so the source\&#39;s own wording may appear. Only a result is released in a studyset. Null on an analysis from before roles, which is read as a result, except on a set the study_schema ingester wrote, which is unclassified. | [optional] [default to undefined]
**relabelled_by** | **string** | The parse_id of the reviewed revision whose relabel verdict set &#x60;role&#x60;; a later parse does not replace a relabelled role. Null while the role is the classifier\&#39;s, whose name and version are in &#x60;metadata.role_source&#x60; (study_schema\&#39;s &#x60;role_source&#x60;). | [optional] [default to undefined]
**outcome** | **string** | Whether anything survived the analysis\&#39;s threshold (study_schema AnalysisOutcome), from the extraction record. The ingester sets it only on results. | [optional] [default to undefined]
**from_prior_study** | **boolean** | The coordinates are quoted from an earlier study, not this one\&#39;s. | [optional] [default to undefined]

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
    role,
    relabelled_by,
    outcome,
    from_prior_study,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
