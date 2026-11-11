# AnalysisQueryAcquisitions

The analysis\'s acquisitions; a number matches when any acquisition\'s does. The voxel size is an acquisition\'s largest dimension.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**modality** | [**AnalysisQueryValue**](AnalysisQueryValue.md) |  | [optional] [default to undefined]
**magnetic_field_strength_tesla** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**repetition_time_seconds** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**echo_time_seconds** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**acquisition_voxel_size_mm** | [**AnalysisQueryRange**](AnalysisQueryRange.md) |  | [optional] [default to undefined]
**device** | [**AnalysisQueryText**](AnalysisQueryText.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryAcquisitions } from './api';

const instance: AnalysisQueryAcquisitions = {
    modality,
    magnetic_field_strength_tesla,
    repetition_time_seconds,
    echo_time_seconds,
    acquisition_voxel_size_mm,
    device,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
