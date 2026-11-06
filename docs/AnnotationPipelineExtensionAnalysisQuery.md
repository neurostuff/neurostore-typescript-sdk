# AnnotationPipelineExtensionAnalysisQuery

Run an analysis query over the annotation\'s studyset and write its result into the notes: `column` (boolean) is true for each analysis the query selects and false for every other, and each of `feature_columns` (string) carries that analysis\'s feature, or null where its record says nothing. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | [**AnalysisQuery**](AnalysisQuery.md) |  | [default to undefined]
**column** | **string** |  | [optional] [default to 'included']
**feature_columns** | **Array&lt;string&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { AnnotationPipelineExtensionAnalysisQuery } from './api';

const instance: AnnotationPipelineExtensionAnalysisQuery = {
    query,
    column,
    feature_columns,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
