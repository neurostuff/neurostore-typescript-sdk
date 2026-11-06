# QueryResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dataset** | **string** |  | [optional] [default to undefined]
**query** | **{ [key: string]: string; }** | The query as it was read, one key per &#x60;$&#x60; parameter given. | [optional] [default to undefined]
**columns** | [**Array&lt;QueryResultColumnsInner&gt;**](QueryResultColumnsInner.md) |  | [optional] [default to undefined]
**rows** | **Array&lt;Array&lt;any&gt;&gt;** | One array per row, in the order of &#x60;columns&#x60;. | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**offset** | **number** |  | [optional] [default to undefined]
**refreshed_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { QueryResult } from './api';

const instance: QueryResult = {
    dataset,
    query,
    columns,
    rows,
    limit,
    offset,
    refreshed_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
