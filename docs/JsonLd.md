# JsonLd

JSON-LD elements for data tracking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**at_context** | [**JsonLdContext**](JsonLdContext.md) |  | [optional] [default to undefined]
**at_id** | **string** | URI of the resource | [optional] [default to undefined]
**at_type** | **string** | One of the NiMADS data types | [optional] [default to undefined]

## Example

```typescript
import { JsonLd } from './api';

const instance: JsonLd = {
    at_context,
    at_id,
    at_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
