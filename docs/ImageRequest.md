# ImageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | **object** | Metadata about image such as software and version used and other relevant data about how the image was produced. | [optional] [default to undefined]
**url** | **string** | URL to image file. | [optional] [default to undefined]
**filename** | **string** | Name of the image file. | [optional] [default to undefined]
**space** | **string** | The template space the image is in (e.g., MNI  | [optional] [default to undefined]
**value_type** | **string** | The values the image represents. For example, T-statistic or Z-statistic, or Betas. | [optional] [default to undefined]
**add_date** | **string** | Date the image was added. | [optional] [readonly] [default to undefined]
**analysis** | **string** |  | [optional] [default to undefined]
**entities** | [**Array&lt;Entity&gt;**](Entity.md) |  | [optional] [default to undefined]
**analysis_name** | **string** |  | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]

## Example

```typescript
import { ImageRequest } from './api';

const instance: ImageRequest = {
    metadata,
    url,
    filename,
    space,
    value_type,
    add_date,
    analysis,
    entities,
    analysis_name,
    id,
    _public,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
