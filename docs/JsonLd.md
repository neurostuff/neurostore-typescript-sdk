# JsonLd

JSON-LD elements for data tracking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**JsonLdContext**](JsonLdContext.md) |  | [optional] [default to undefined]
**id** | **string** | URI of the resource | [optional] [default to undefined]
**type** | **string** | One of the NiMADS data types | [optional] [default to undefined]

## Example

```typescript
import { JsonLd } from './api';

const instance: JsonLd = {
    context,
    id,
    type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
