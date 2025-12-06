# ImageBase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | **object** | Metadata about image such as software and version used and other relevant data about how the image was produced. | [optional] [default to undefined]
**url** | **string** | URL to image file. | [optional] [default to undefined]
**filename** | **string** | Name of the image file. | [optional] [default to undefined]
**space** | **string** | The template space the image is in (e.g., MNI  | [optional] [default to undefined]
**value_type** | **string** | The values the image represents. For example, T-statistic or Z-statistic, or Betas. | [optional] [default to undefined]
**add_date** | **string** | Date the image was added. | [optional] [readonly] [default to undefined]

## Example

```typescript
import { ImageBase } from './api';

const instance: ImageBase = {
    metadata,
    url,
    filename,
    space,
    value_type,
    add_date,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
