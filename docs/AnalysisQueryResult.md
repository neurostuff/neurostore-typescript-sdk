# AnalysisQueryResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **{ [key: string]: any; }** | The query in canonical form, every criterion as any/all/none lists. | [optional] [default to undefined]
**counts** | [**AnalysisQueryResultCounts**](AnalysisQueryResultCounts.md) |  | [optional] [default to undefined]
**searched** | [**AnalysisQueryResultSearched**](AnalysisQueryResultSearched.md) |  | [optional] [default to undefined]
**funnel** | [**Array&lt;AnalysisQueryResultFunnelInner&gt;**](AnalysisQueryResultFunnelInner.md) | With &#x60;funnel&#x60;, the criteria in order, each with what remains after it. | [optional] [default to undefined]
**results** | [**Array&lt;AnalysisQueryResultResultsInner&gt;**](AnalysisQueryResultResultsInner.md) |  | [optional] [default to undefined]
**study_ids** | **Array&lt;string&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResult } from './api';

const instance: AnalysisQueryResult = {
    query,
    counts,
    searched,
    funnel,
    results,
    study_ids,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
