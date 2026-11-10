# AnalysisQueryResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**AnalysisQueryResultMetadata**](AnalysisQueryResultMetadata.md) |  | [optional] [default to undefined]
**query** | **{ [key: string]: any; }** | The query in canonical form: a normalized criterion as ids, text, all, none, descendants, when_unmapped and when_silent, every other as any/all/none lists.  | [optional] [default to undefined]
**searched** | [**AnalysisQueryResultSearched**](AnalysisQueryResultSearched.md) |  | [optional] [default to undefined]
**funnel** | [**Array&lt;AnalysisQueryResultFunnelInner&gt;**](AnalysisQueryResultFunnelInner.md) | With &#x60;funnel&#x60;, the criteria in order, each with what remains after it. | [optional] [default to undefined]
**results** | [**Array&lt;AnalysisQueryResultResultsInner&gt;**](AnalysisQueryResultResultsInner.md) | The page\&#39;s studies, in order of paper, each with its selected analyses. | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResult } from './api';

const instance: AnalysisQueryResult = {
    metadata,
    query,
    searched,
    funnel,
    results,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
