# AnalysisCommon

attributes common between request and return objects

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**study** | **string** |  | [optional] [default to undefined]
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
import { AnalysisCommon } from './api';

const instance: AnalysisCommon = {
    study,
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
