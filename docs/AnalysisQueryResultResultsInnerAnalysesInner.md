# AnalysisQueryResultResultsInnerAnalysesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**matched_by** | **{ [key: string]: string; }** | How the analysis matched each normalized criterion, by its path (&#x60;medical_condition&#x60;, &#x60;or[0].task&#x60;): by id, by text, as unmapped or as silent (under &#x60;include&#x60;). Absent where a mapped analysis matched only through &#x60;none&#x60;.  | [optional] [default to undefined]
**role** | **string** | With &#x60;features&#x60;, the analysis\&#39;s coordinate role (the &#x60;role&#x60; criterion), which a review can change apart from its features.  | [optional] [default to undefined]
**has_coordinates** | **boolean** | With &#x60;features&#x60;, whether the analysis has coordinates. | [optional] [default to undefined]
**config_id** | **string** | With &#x60;features&#x60;, the pipeline config of the record they were read from. | [optional] [default to undefined]
**updated_at** | **string** | With &#x60;features&#x60;, when they were last written. Every re-ingest of the paper rewrites them, changed or not.  | [optional] [default to undefined]
**features** | [**AnalysisFeatures**](AnalysisFeatures.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryResultResultsInnerAnalysesInner } from './api';

const instance: AnalysisQueryResultResultsInnerAnalysesInner = {
    id,
    name,
    matched_by,
    role,
    has_coordinates,
    config_id,
    updated_at,
    features,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
