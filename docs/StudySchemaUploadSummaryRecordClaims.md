# StudySchemaUploadSummaryRecordClaims


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **number** |  | [optional] [default to undefined]
**matched** | **number** |  | [optional] [default to undefined]
**rejected_paths** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**unkeyed_entities** | **Array&lt;string&gt;** | Record entities with no key to identify them by. | [optional] [default to undefined]
**parked_entities** | [**Array&lt;StudySchemaSetAside&gt;**](StudySchemaSetAside.md) | Set-aside entities: positional keys, or keys no stored parse holds (resolved later by a parse that holds them; see set_aside_resolved).  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummaryRecordClaims } from './api';

const instance: StudySchemaUploadSummaryRecordClaims = {
    created,
    matched,
    rejected_paths,
    unkeyed_entities,
    parked_entities,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
