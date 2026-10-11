# StudySchemaUploadSummarySkeletonOrphanedClaimsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **string** | The superseded analysis\&#39;s key. | [optional] [default to undefined]
**_class** | **string** | The entity class. | [optional] [default to undefined]
**entity_id** | **string** |  | [optional] [default to undefined]
**claims** | **number** | How many claims the entity holds. | [optional] [default to undefined]
**reason** | **string** | Why the claims stayed. not_carried: the upload is a revision and the analysis is neither linked nor split or merged. alias_conflict: an original parse, and the key is in alias_conflicts. no_successor: an original parse with no successor.  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummarySkeletonOrphanedClaimsInner } from './api';

const instance: StudySchemaUploadSummarySkeletonOrphanedClaimsInner = {
    key,
    _class,
    entity_id,
    claims,
    reason,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
