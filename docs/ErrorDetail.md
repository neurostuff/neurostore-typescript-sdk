# ErrorDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**field** | **string** | Field name that caused the error | [optional] [default to undefined]
**code** | **string** | Machine-readable error code | [default to undefined]
**message** | **string** | Human-readable error message | [default to undefined]
**context** | **{ [key: string]: any; }** | Additional error context | [optional] [default to undefined]

## Example

```typescript
import { ErrorDetail } from './api';

const instance: ErrorDetail = {
    field,
    code,
    message,
    context,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
