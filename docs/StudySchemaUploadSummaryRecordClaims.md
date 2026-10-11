# StudySchemaUploadSummaryRecordClaims


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **number** |  | [optional] [default to undefined]
**matched** | **number** |  | [optional] [default to undefined]
**rejected_paths** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**entities** | [**StudySchemaUploadSummaryRecordClaimsEntities**](StudySchemaUploadSummaryRecordClaimsEntities.md) |  | [optional] [default to undefined]
**unlocated** | **Array&lt;string&gt;** | Paths of analysis or coordinate-set items with no cells or spans to locate them by; they are not stored as entities. | [optional] [default to undefined]
**unidentified** | **Array&lt;string&gt;** | Paths of entity lists that are not lists, and of their items that are not objects; not stored as entities. | [optional] [default to undefined]
**duplicates** | **Array&lt;string&gt;** | Paths of items whose hash an earlier item of the record already has (one analysis read twice from the same cells under the same name); not stored. | [optional] [default to undefined]
**rename_candidates** | [**Array&lt;StudySchemaRenameCandidate&gt;**](StudySchemaRenameCandidate.md) | Entities the record names differently from a stored entity in the same place. They are linked as renamed_by_extractor candidates; claims stay on the old entity until a curator links them.  | [optional] [default to undefined]
**released_aliases** | **Array&lt;string&gt;** | Paths of new items whose hash was an alias of another entity; the alias is dropped. | [optional] [default to undefined]
**parked_entities** | [**Array&lt;StudySchemaSetAside&gt;**](StudySchemaSetAside.md) | Set-aside entities: positional keys, or keys no stored parse holds (resolved later by a parse that holds them; see set_aside_resolved).  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummaryRecordClaims } from './api';

const instance: StudySchemaUploadSummaryRecordClaims = {
    created,
    matched,
    rejected_paths,
    entities,
    unlocated,
    unidentified,
    duplicates,
    rename_candidates,
    released_aliases,
    parked_entities,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
