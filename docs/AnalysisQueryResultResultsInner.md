# AnalysisQueryResultResultsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**analysis** | **string** |  | [optional] [default to undefined]
**study** | **string** |  | [optional] [default to undefined]
**base_study** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**matched_by** | **{ [key: string]: string; }** | How the analysis matched each normalized criterion, by its path (&#x60;medical_condition&#x60;, &#x60;or[0].task&#x60;): by id, by text, as unmapped or as silent (under &#x60;include&#x60;). Absent where a mapped analysis matched only through &#x60;none&#x60;.  | [optional] [default to undefined]
**features** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResultResultsInner } from './api';

const instance: AnalysisQueryResultResultsInner = {
    analysis,
    study,
    base_study,
    name,
    matched_by,
    features,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
