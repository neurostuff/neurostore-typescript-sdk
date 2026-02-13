# WriteableResourceAttributes

common resource attributes

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]

## Example

```typescript
import { WriteableResourceAttributes } from './api';

const instance: WriteableResourceAttributes = {
    id,
    _public,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
