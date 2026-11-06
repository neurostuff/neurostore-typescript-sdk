# AnalysisTermListResultsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **string** |  | [optional] [default to undefined]
**label** | **string** |  | [optional] [default to undefined]
**parent** | **string** | The term directly above it (a task\&#39;s or a contrast\&#39;s family). | [optional] [default to undefined]
**children** | **Array&lt;string&gt;** | The terms directly under it. | [optional] [default to undefined]
**synonyms** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**analyses** | **number** |  | [optional] [default to undefined]
**base_studies** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisTermListResultsInner } from './api';

const instance: AnalysisTermListResultsInner = {
    value,
    label,
    parent,
    children,
    synonyms,
    analyses,
    base_studies,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
