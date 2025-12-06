# AnalysisBase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | A name of the contrast being performed. | [optional] [default to undefined]
**description** | **string** | A long form description of how the contrast was performed | [optional] [default to undefined]
**weights** | **Array&lt;number&gt;** | Weight applied to each condition, must be the same length as the conditions attribute. | [optional] [default to undefined]

## Example

```typescript
import { AnalysisBase } from './api';

const instance: AnalysisBase = {
    name,
    description,
    weights,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
