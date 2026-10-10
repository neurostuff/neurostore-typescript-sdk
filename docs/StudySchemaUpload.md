# StudySchemaUpload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**coordinate_parse** | **{ [key: string]: any; }** | A study_schema CoordinateParse (neuroimaging-paper-parse); a revision when revision_of is set. | [optional] [default to undefined]
**record** | **{ [key: string]: any; }** | A study_schema extraction record (neuroimaging-study-extraction). | [optional] [default to undefined]
**parsed_paper** | **{ [key: string]: any; }** | The ParsedPaper the parse read, for table captions and the bibliography. | [optional] [default to undefined]
**parse_id** | **string** | For a record uploaded alone, the parse_id of the stored parse it read. | [optional] [default to undefined]
**base_study_id** | **string** | The base study; otherwise found by the parse header\&#39;s identifiers. | [optional] [default to undefined]
**pipeline** | [**StudySchemaUploadPipeline**](StudySchemaUploadPipeline.md) |  | [optional] [default to undefined]

## Example

```typescript
import { StudySchemaUpload } from './api';

const instance: StudySchemaUpload = {
    coordinate_parse,
    record,
    parsed_paper,
    parse_id,
    base_study_id,
    pipeline,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
