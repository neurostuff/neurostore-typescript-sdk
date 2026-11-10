# AnalysisQueryResultResultsInnerAnalysesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**matched_by** | **{ [key: string]: string; }** | How the analysis matched each normalized criterion, by its path (&#x60;medical_condition&#x60;, &#x60;or[0].task&#x60;): by id, by text, as unmapped or as silent (under &#x60;include&#x60;). Absent where a mapped analysis matched only through &#x60;none&#x60;.  | [optional] [default to undefined]
**features** | **{ [key: string]: any; }** | Only when &#x60;detail&#x60; is &#x60;features&#x60;. | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResultResultsInnerAnalysesInner } from './api';

const instance: AnalysisQueryResultResultsInnerAnalysesInner = {
    id,
    name,
    matched_by,
    features,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
