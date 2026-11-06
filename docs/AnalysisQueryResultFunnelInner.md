# AnalysisQueryResultFunnelInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**criterion** | **string** |  | [optional] [default to undefined]
**analyses** | **number** |  | [optional] [default to undefined]
**base_studies** | **number** |  | [optional] [default to undefined]
**dropped** | **number** |  | [optional] [default to undefined]
**silent** | **number** | Analyses left by the criteria before this one whose record says nothing on it. | [optional] [default to undefined]
**unmapped** | **number** | For a normalized criterion, the analyses left by the criteria before this one whose record states the feature but maps none of it.  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResultFunnelInner } from './api';

const instance: AnalysisQueryResultFunnelInner = {
    criterion,
    analyses,
    base_studies,
    dropped,
    silent,
    unmapped,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
