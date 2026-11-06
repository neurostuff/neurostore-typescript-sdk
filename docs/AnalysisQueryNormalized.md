# AnalysisQueryNormalized

Text (a pattern, or a list of them, any of which may match), or ids and text. `ids` and `text` are any-of, and either may match; `all` needs every one and `none` refuses each. `when_unmapped` decides an analysis whose record states the feature but maps none of it: `exclude` (the default), `include`, or `text`, matching it by its wording alone, so a criterion without text excludes it. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ids** | [**AnalysisQueryStrings**](AnalysisQueryStrings.md) |  | [optional] [default to undefined]
**text** | [**AnalysisQueryStrings**](AnalysisQueryStrings.md) |  | [optional] [default to undefined]
**all** | [**AnalysisQueryTerms**](AnalysisQueryTerms.md) |  | [optional] [default to undefined]
**none** | [**AnalysisQueryTerms**](AnalysisQueryTerms.md) |  | [optional] [default to undefined]
**descendants** | **boolean** | Whether an id also matches the terms below it in its vocabulary. | [optional] [default to true]
**when_unmapped** | **string** |  | [optional] [default to WhenUnmappedEnum_Exclude]
**when_silent** | [**AnalysisQueryWhenSilent**](AnalysisQueryWhenSilent.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryNormalized } from './api';

const instance: AnalysisQueryNormalized = {
    ids,
    text,
    all,
    none,
    descendants,
    when_unmapped,
    when_silent,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
