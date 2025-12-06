# AnalysisCommon

attributes common between request and return objects

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**study** | **string** |  | [optional] [default to undefined]
**table_id** | **string** |  | [optional] [default to undefined]
**entities** | [**Array&lt;Entity&gt;**](Entity.md) |  | [optional] [default to undefined]
**order** | **number** |  | [optional] [default to undefined]
**metadata** | **object** |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisCommon } from './api';

const instance: AnalysisCommon = {
    study,
    table_id,
    entities,
    order,
    metadata,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
