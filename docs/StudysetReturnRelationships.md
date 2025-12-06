# StudysetReturnRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**studyset_studies** | [**Array&lt;StudysetReturnRelationshipsStudysetStudiesInner&gt;**](StudysetReturnRelationshipsStudysetStudiesInner.md) | Association records for studies in this studyset (includes stub UUIDs for mapping). | [optional] [default to undefined]
**studies** | [**StudysetReturnRelationshipsStudies**](StudysetReturnRelationshipsStudies.md) |  | [optional] [default to undefined]

## Example

```typescript
import { StudysetReturnRelationships } from './api';

const instance: StudysetReturnRelationships = {
    studyset_studies,
    studies,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
