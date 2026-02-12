# PointReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**coordinates** | **Array&lt;number&gt;** | Location of the significant coordinate in three dimensional space. | [optional] [default to undefined]
**space** | **string** | Template space used to determine coordinate Examples include TAL or MNI. | [optional] [default to undefined]
**kind** | **string** | Method of how point was derived (e.g., center of mass) | [optional] [default to undefined]
**label_id** | **string** | If the point is associated with an image, this is the value the point takes in that image. | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**image** | **string** |  | [optional] [default to undefined]
**values** | [**PointRelationshipsValues**](PointRelationshipsValues.md) |  | [optional] [default to undefined]
**x** | **number** |  | [optional] [default to undefined]
**y** | **number** |  | [optional] [default to undefined]
**z** | **number** |  | [optional] [default to undefined]
**entities** | [**Array&lt;Entity&gt;**](Entity.md) |  | [optional] [default to undefined]
**analysis** | **string** |  | [optional] [default to undefined]
**cluster_size** | **number** | size of the cluster in cubic millimeters | [optional] [default to undefined]
**subpeak** | **boolean** | whether the reported peak is the max-peak statistic or a sub-maxmimal peak. | [optional] [default to undefined]
**deactivation** | **boolean** | wheather the coordinate represents an decrease in activation relative to a baseline | [optional] [default to undefined]
**order** | **number** | determines the row to display the coordinate | [optional] [default to undefined]

## Example

```typescript
import { PointReturn } from './api';

const instance: PointReturn = {
    coordinates,
    space,
    kind,
    label_id,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    image,
    values,
    x,
    y,
    z,
    entities,
    analysis,
    cluster_size,
    subpeak,
    deactivation,
    order,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
