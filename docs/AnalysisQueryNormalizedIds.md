# AnalysisQueryNormalizedIds

Ids (an id, or a list of them, any of which may match), as analysis-query-normalized without text. An analysis whose record states the feature but maps none of it is excluded unless `when_unmapped` is `include`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ids** | [**AnalysisQueryStrings**](AnalysisQueryStrings.md) |  | [optional] [default to undefined]
**all** | [**AnalysisQueryIds**](AnalysisQueryIds.md) |  | [optional] [default to undefined]
**none** | [**AnalysisQueryIds**](AnalysisQueryIds.md) |  | [optional] [default to undefined]
**descendants** | **boolean** | Whether an id also matches the terms below it in its vocabulary. | [optional] [default to true]
**when_unmapped** | **string** |  | [optional] [default to WhenUnmappedEnum_Exclude]
**when_silent** | [**AnalysisQueryWhenSilent**](AnalysisQueryWhenSilent.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryNormalizedIds } from './api';

const instance: AnalysisQueryNormalizedIds = {
    ids,
    all,
    none,
    descendants,
    when_unmapped,
    when_silent,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
