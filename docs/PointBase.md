# PointBase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**coordinates** | **Array&lt;number&gt;** | Location of the significant coordinate in three dimensional space. | [optional] [default to undefined]
**space** | **string** | Template space used to determine coordinate Examples include TAL or MNI. | [optional] [default to undefined]
**kind** | **string** | Method of how point was derived (e.g., center of mass) | [optional] [default to undefined]
**label_id** | **string** | If the point is associated with an image, this is the value the point takes in that image. | [optional] [default to undefined]

## Example

```typescript
import { PointBase } from './api';

const instance: PointBase = {
    coordinates,
    space,
    kind,
    label_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
