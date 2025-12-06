# StudyRequest


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
**analyses** | [**StudyRequestRelationshipsAnalyses**](StudyRequestRelationshipsAnalyses.md) |  | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**pmcid** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { StudyRequest } from './api';

const instance: StudyRequest = {
    doi,
    name,
    metadata,
    description,
    publication,
    pmid,
    authors,
    year,
    analyses,
    id,
    _public,
    pmcid,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
