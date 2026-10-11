# StudySchemaUploadSummaryRecordConditionConflictsInnerCellsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**term** | **string** |  | [optional] [default to undefined]
**level** | **string** | The cell\&#39;s level, or its label when it has no level. | [optional] [default to undefined]
**reason** | **string** | both_directions: the cell is listed both positive and negative. shared_name: two cells would name the same condition.  | [optional] [default to undefined]
**name** | **string** | The condition name the cells share. Only for shared_name. | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUploadSummaryRecordConditionConflictsInnerCellsInner } from './api';

const instance: StudySchemaUploadSummaryRecordConditionConflictsInnerCellsInner = {
    term,
    level,
    reason,
    name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
