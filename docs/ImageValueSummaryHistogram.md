# ImageValueSummaryHistogram

Equal-width bins over [min, max]. Bin edges are implied by the bounds and the length of counts.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**min** | **number** |  | [optional] [default to undefined]
**max** | **number** |  | [optional] [default to undefined]
**bin_width** | **number** |  | [optional] [default to undefined]
**counts** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**underflow** | **number** | Values below min, clipped out of the binned range. | [optional] [default to undefined]
**overflow** | **number** | Values above max, clipped out of the binned range. | [optional] [default to undefined]

## Example

```typescript
import { ImageValueSummaryHistogram } from './api';

const instance: ImageValueSummaryHistogram = {
    min,
    max,
    bin_width,
    counts,
    underflow,
    overflow,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
