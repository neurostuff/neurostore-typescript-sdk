# AnalysisQueryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | [**AnalysisQuery**](AnalysisQuery.md) |  | [default to undefined]
**limit** | **number** | How many selected analyses to list; counts and study_ids cover them all. | [optional] [default to 100]
**funnel** | **boolean** | Also return &#x60;searched&#x60; and &#x60;funnel&#x60;: what each criterion in turn keeps and drops, and how many analyses it finds silent. It counts once per criterion, so it costs most when criteria keep most analyses.  | [optional] [default to false]

## Example

```typescript
import { AnalysisQueryRequest } from './api';

const instance: AnalysisQueryRequest = {
    query,
    limit,
    funnel,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
