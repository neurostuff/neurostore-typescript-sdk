# BaseStudiesPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | **object** |  | [optional] [default to undefined]
**versions** | [**Array&lt;BaseStudyVersionsInner&gt;**](BaseStudyVersionsInner.md) |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**publication** | **string** |  | [optional] [default to undefined]
**doi** | **string** |  | [optional] [default to undefined]
**pmid** | **string** |  | [optional] [default to undefined]
**authors** | **string** |  | [optional] [default to undefined]
**year** | **number** |  | [optional] [default to undefined]
**level** | **string** |  | [optional] [default to undefined]
**is_oa** | **boolean** |  | [optional] [default to undefined]
**pmcid** | **string** |  | [optional] [default to undefined]
**neurovault_id** | [**BaseStudyNeurovaultId**](BaseStudyNeurovaultId.md) |  | [optional] [default to undefined]

## Example

```typescript
import { BaseStudiesPostRequest } from './api';

const instance: BaseStudiesPostRequest = {
    metadata,
    versions,
    name,
    description,
    publication,
    doi,
    pmid,
    authors,
    year,
    level,
    is_oa,
    pmcid,
    neurovault_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
