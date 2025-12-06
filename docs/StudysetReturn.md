# StudysetReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Descriptive and human readable name of the studyset. | [optional] [default to undefined]
**description** | **string** | A longform description of the studyset. | [optional] [default to undefined]
**publication** | **string** | The journal/source the studyset is connected to if the studyset was published. | [optional] [default to undefined]
**doi** | **string** | A DOI connected to the published studyset (may change to being automatically created so each studyset connected to a successful meta-analysis gets a DOI). | [optional] [default to undefined]
**pmid** | **string** | If the article connected to the studyset was published on PubMed, then link the ID here. | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**source** | **string** |  | [optional] [default to undefined]
**source_id** | **string** |  | [optional] [default to undefined]
**source_updated_at** | **string** |  | [optional] [readonly] [default to undefined]
**studies** | [**StudysetReturnRelationshipsStudies**](StudysetReturnRelationshipsStudies.md) |  | [optional] [default to undefined]
**level** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { StudysetReturn } from './api';

const instance: StudysetReturn = {
    name,
    description,
    publication,
    doi,
    pmid,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    source,
    source_id,
    source_updated_at,
    studies,
    level,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
