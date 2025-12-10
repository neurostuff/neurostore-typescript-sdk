# StudysetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Descriptive and human readable name of the studyset. | [optional] [default to undefined]
**description** | **string** | A longform description of the studyset. | [optional] [default to undefined]
**publication** | **string** | The journal/source the studyset is connected to if the studyset was published. | [optional] [default to undefined]
**doi** | **string** | A DOI connected to the published studyset (may change to being automatically created so each studyset connected to a successful meta-analysis gets a DOI). | [optional] [default to undefined]
**pmid** | **string** | If the article connected to the studyset was published on PubMed, then link the ID here. | [optional] [default to undefined]
**studies** | [**Array&lt;StudysetRequestRelationshipsStudiesInner&gt;**](StudysetRequestRelationshipsStudiesInner.md) | Accepts study IDs or objects containing an ID and an optional curation stub UUID used to keep curation/extraction alignment.  | [optional] [default to undefined]
**curation_stub_map** | **{ [key: string]: string; }** | Accepts a map of each study ID to the curation stub UUID used to keep curation/extraction alignment.  | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**level** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { StudysetRequest } from './api';

const instance: StudysetRequest = {
    name,
    description,
    publication,
    doi,
    pmid,
    studies,
    curation_stub_map,
    id,
    _public,
    level,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
