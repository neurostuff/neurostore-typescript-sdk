# BaseStudyVersionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**doi** | **string** | Digital object identifier of the study. | [optional] [default to undefined]
**name** | **string** | Title of the study. | [optional] [default to undefined]
**metadata** | **object** | Metadata associated with the study not covered by the other study attributes. | [optional] [default to undefined]
**description** | **string** | Long form description of the study, typically the abstract. | [optional] [default to undefined]
**publication** | **string** | The journal/place of publication for the study. | [optional] [default to undefined]
**pmid** | **string** | If the study was published on PubMed, place the PubMed ID here. | [optional] [default to undefined]
**authors** | **string** | The authors on the publication of this study. | [optional] [default to undefined]
**year** | **number** | The year this study was published. | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**source** | **string** |  | [optional] [default to undefined]
**source_id** | **string** |  | [optional] [default to undefined]
**source_updated_at** | **string** |  | [optional] [readonly] [default to undefined]
**analyses** | [**StudyReturnRelationshipsAnalyses**](StudyReturnRelationshipsAnalyses.md) |  | [optional] [default to undefined]
**tables** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**studysets** | [**Array&lt;StudyReturnAllOfStudysets&gt;**](StudyReturnAllOfStudysets.md) |  | [optional] [default to undefined]
**has_coordinates** | **boolean** |  | [optional] [default to undefined]
**has_images** | **boolean** |  | [optional] [default to undefined]
**base_study** | **string** |  | [optional] [default to undefined]
**pmcid** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { BaseStudyVersionsInner } from './api';

const instance: BaseStudyVersionsInner = {
    doi,
    name,
    metadata,
    description,
    publication,
    pmid,
    authors,
    year,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    source,
    source_id,
    source_updated_at,
    analyses,
    tables,
    studysets,
    has_coordinates,
    has_images,
    base_study,
    pmcid,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
