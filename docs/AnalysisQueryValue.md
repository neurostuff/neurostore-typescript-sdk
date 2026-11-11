# AnalysisQueryValue

Values matched whole: a value, a list of values (any of them), or any/all/none lists. Unlike a text criterion, no pattern and no minimum length. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**any** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**all** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**none** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**when_silent** | [**AnalysisQueryWhenSilent**](AnalysisQueryWhenSilent.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryValue } from './api';

const instance: AnalysisQueryValue = {
    any,
    all,
    none,
    when_silent,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
