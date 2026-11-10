# AnalysisQueryAcquisition

The analysis\'s acquisitions; a criterion on a number matches when any acquisition\'s does. Field strength in tesla, repetition and echo time in seconds, voxel size as the largest dimension in millimetres. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**modality** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]
**field_strength** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**repetition_time** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**echo_time** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**voxel_size** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**scanner** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryAcquisition } from './api';

const instance: AnalysisQueryAcquisition = {
    modality,
    field_strength,
    repetition_time,
    echo_time,
    voxel_size,
    scanner,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
