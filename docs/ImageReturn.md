# ImageReturn


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
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]

## Example

```typescript
import { ImageReturn } from './api';

const instance: ImageReturn = {
    metadata,
    url,
    filename,
    space,
    value_type,
    add_date,
    analysis,
    entities,
    analysis_name,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
