# ImageValueSummary

Distribution statistics for the image\'s voxel values, computed once and stored. Present only when image_value_summary=true is requested, and null when the image has never been summarized. Counts cover every voxel in the file; the distribution fields (min/max/mean/std, percentiles, histogram) cover only the finite, non-zero voxels, because neuroimaging maps store their background as zero or nan.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **string** | SUCCESS when the numbers below are populated, FAILURE when the image could not be read. | [optional] [default to undefined]
**error** | **string** | Why the last attempt failed, when status is not SUCCESS. | [optional] [default to undefined]
**summarizer_version** | **number** | Which version of the summarizer produced these numbers. | [optional] [default to undefined]
**computed_at** | **string** |  | [optional] [default to undefined]
**source_sha256** | **string** | SHA-256 of the file that was summarized, so a client can tell whether the numbers still describe the file at url. | [optional] [default to undefined]
**source_bytes** | **number** |  | [optional] [default to undefined]
**n_voxels** | **number** | Total voxels in the file; the denominator for fraction_nan and fraction_zero. | [optional] [default to undefined]
**n_values** | **number** | Finite, non-zero voxels; the n behind the distribution fields and the denominator for fraction_negative. | [optional] [default to undefined]
**fraction_nan** | **number** | Non-finite (nan or inf) voxels over n_voxels. | [optional] [default to undefined]
**fraction_zero** | **number** | Exactly-zero voxels over n_voxels. | [optional] [default to undefined]
**fraction_negative** | **number** | Negative voxels over n_values. A z or t map with a fraction near zero here is either one-sided or mislabelled. | [optional] [default to undefined]
**min** | **number** |  | [optional] [default to undefined]
**max** | **number** |  | [optional] [default to undefined]
**mean** | **number** |  | [optional] [default to undefined]
**std** | **number** |  | [optional] [default to undefined]
**percentiles** | **{ [key: string]: number | null; }** | Percentile value keyed by probe, e.g. {\&quot;0.1\&quot;: -5.2, \&quot;1\&quot;: -3.1, ... \&quot;99.9\&quot;: 5.8}. | [optional] [default to undefined]
**histogram** | [**ImageValueSummaryHistogram**](ImageValueSummaryHistogram.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ImageValueSummary } from './api';

const instance: ImageValueSummary = {
    status,
    error,
    summarizer_version,
    computed_at,
    source_sha256,
    source_bytes,
    n_voxels,
    n_values,
    fraction_nan,
    fraction_zero,
    fraction_negative,
    min,
    max,
    mean,
    std,
    percentiles,
    histogram,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
