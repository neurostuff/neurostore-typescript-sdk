# StudysetRequestRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**studies** | [**Array&lt;StudysetRequestRelationshipsStudiesInner&gt;**](StudysetRequestRelationshipsStudiesInner.md) | Accepts study IDs or objects containing an ID and an optional curation stub UUID used to keep curation/extraction alignment.  | [optional] [default to undefined]
**curation_stub_map** | **{ [key: string]: string; }** | Accepts a map of each study ID to the curation stub UUID used to keep curation/extraction alignment.  | [optional] [default to undefined]

## Example

```typescript
import { StudysetRequestRelationships } from './api';

const instance: StudysetRequestRelationships = {
    studies,
    curation_stub_map,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
