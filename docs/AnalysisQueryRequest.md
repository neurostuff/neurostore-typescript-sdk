# AnalysisQueryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | [**AnalysisQuery**](AnalysisQuery.md) |  | [default to undefined]
**page** | **number** | Which page of studies to list, in order of paper. | [optional] [default to 1]
**page_size** | **number** | How many studies a page lists, each with all its selected analyses; 0 lists none.  | [optional] [default to 20]
**paginate** | **boolean** | False lists every selected study, whatever &#x60;page&#x60; and &#x60;page_size&#x60; say. | [optional] [default to true]
**detail** | **string** | How much each listed study carries: &#x60;studies&#x60; only its ids, &#x60;analyses&#x60; also its selected analyses\&#39; ids, names and matches, &#x60;features&#x60; also their features. With &#x60;paginate: false&#x60;, &#x60;studies&#x60; lists every selected study\&#39;s id at once.  | [optional] [default to DetailEnum_Features]
**base_study_ids** | **Array&lt;string&gt;** | Only the analyses of these papers. The counts, results and funnel cover the same restricted set, so an empty query lists every analysis with features that these papers have.  | [optional] [default to undefined]
**study_ids** | **Array&lt;string&gt;** | Only the analyses of these studies (the pipeline studies the results name). With &#x60;base_study_ids&#x60;, an analysis must be in both.  | [optional] [default to undefined]
**funnel** | **boolean** | Also return &#x60;searched&#x60; and &#x60;funnel&#x60;: what each criterion in turn keeps and drops, and how many analyses it finds silent. It counts once per criterion, so it costs most when criteria keep most analyses.  | [optional] [default to false]

## Example

```typescript
import { AnalysisQueryRequest } from './api';

const instance: AnalysisQueryRequest = {
    query,
    page,
    page_size,
    paginate,
    detail,
    base_study_ids,
    study_ids,
    funnel,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
