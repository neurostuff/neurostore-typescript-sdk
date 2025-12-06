# PointCommon


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**analysis** | **string** |  | [optional] [default to undefined]
**cluster_size** | **number** | size of the cluster in cubic millimeters | [optional] [default to undefined]
**subpeak** | **boolean** | whether the reported peak is the max-peak statistic or a sub-maxmimal peak. | [optional] [default to undefined]
**deactivation** | **boolean** | wheather the coordinate represents an decrease in activation relative to a baseline | [optional] [default to undefined]
**order** | **number** | determines the row to display the coordinate | [optional] [default to undefined]

## Example

```typescript
import { PointCommon } from './api';

const instance: PointCommon = {
    analysis,
    cluster_size,
    subpeak,
    deactivation,
    order,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
