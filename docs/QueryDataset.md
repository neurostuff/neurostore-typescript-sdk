# QueryDataset


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**key** | **Array&lt;string&gt;** | The columns that identify a row. | [optional] [default to undefined]
**columns** | [**Array&lt;QueryDatasetColumnsInner&gt;**](QueryDatasetColumnsInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { QueryDataset } from './api';

const instance: QueryDataset = {
    name,
    description,
    key,
    columns,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
