# AnalysisQueryMedicalConditionOneOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ids** | [**AnalysisQueryStrings**](AnalysisQueryStrings.md) |  | [optional] [default to undefined]
**text** | [**AnalysisQueryStrings**](AnalysisQueryStrings.md) |  | [optional] [default to undefined]
**all** | [**AnalysisQueryTerms**](AnalysisQueryTerms.md) |  | [optional] [default to undefined]
**none** | [**AnalysisQueryTerms**](AnalysisQueryTerms.md) |  | [optional] [default to undefined]
**descendants** | **boolean** | Whether an id also matches the terms below it in its vocabulary. | [optional] [default to true]
**role** | [**AnalysisQueryMedicalConditionOneOfRole**](AnalysisQueryMedicalConditionOneOfRole.md) |  | [optional] [default to undefined]
**when_unmapped** | **string** |  | [optional] [default to WhenUnmappedEnum_Exclude]
**when_silent** | [**AnalysisQueryWhenSilent**](AnalysisQueryWhenSilent.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AnalysisQueryMedicalConditionOneOf } from './api';

const instance: AnalysisQueryMedicalConditionOneOf = {
    ids,
    text,
    all,
    none,
    descendants,
    role,
    when_unmapped,
    when_silent,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
