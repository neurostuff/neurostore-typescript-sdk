# AnalysisQueryDetails

A connectivity analysis\'s details; regions by their names.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connectivity_method** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**inference_target** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**seed_regions** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**target_regions** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryDetails } from './api';

const instance: AnalysisQueryDetails = {
    connectivity_method,
    inference_target,
    seed_regions,
    target_regions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
