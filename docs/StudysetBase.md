# StudysetBase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Descriptive and human readable name of the studyset. | [optional] [default to undefined]
**description** | **string** | A longform description of the studyset. | [optional] [default to undefined]
**publication** | **string** | The journal/source the studyset is connected to if the studyset was published. | [optional] [default to undefined]
**doi** | **string** | A DOI connected to the published studyset (may change to being automatically created so each studyset connected to a successful meta-analysis gets a DOI). | [optional] [default to undefined]
**pmid** | **string** | If the article connected to the studyset was published on PubMed, then link the ID here. | [optional] [default to undefined]

## Example

```typescript
import { StudysetBase } from './api';

const instance: StudysetBase = {
    name,
    description,
    publication,
    doi,
    pmid,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
