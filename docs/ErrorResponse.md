# ErrorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **number** | HTTP status code | [default to undefined]
**title** | **string** | Short, human-readable summary | [default to undefined]
**detail** | **string** | Human-readable explanation | [default to undefined]
**type** | **string** | URI reference for error type | [optional] [default to 'about:blank']
**instance** | **string** | URI reference for specific occurrence | [optional] [default to undefined]
**errors** | [**Array&lt;ErrorDetail&gt;**](ErrorDetail.md) | Field-specific validation errors | [optional] [default to undefined]
**timestamp** | **string** | ISO 8601 timestamp | [default to undefined]
**request_id** | **string** | Unique request identifier | [default to undefined]

## Example

```typescript
import { ErrorResponse } from './api';

const instance: ErrorResponse = {
    status,
    title,
    detail,
    type,
    instance,
    errors,
    timestamp,
    request_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
