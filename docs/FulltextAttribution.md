# FulltextAttribution

What to credit when passing the text on.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **string** |  | [optional] [default to undefined]
**authors** | **string** |  | [optional] [default to undefined]
**year** | **number** |  | [optional] [default to undefined]
**publication** | **string** |  | [optional] [default to undefined]
**doi** | **string** |  | [optional] [default to undefined]
**license** | **string** | A value of study_schema\&#39;s &#x60;LicenseId&#x60; (https://github.com/neurostuff/study_schema/blob/main/src/study_schema/linkml/neuroimaging-study-storage/license.yaml), such as &#x60;cc_by&#x60; or &#x60;all_rights_reserved&#x60;; any other value is refused. The values it annotates &#x60;redistributable&#x60; let a text be passed on with attribution. | [optional] [default to undefined]
**license_statement** | **string** | The licence as its source stated it (a licence URL, name or copyright line). | [optional] [default to undefined]

## Example

```typescript
import { FulltextAttribution } from './api';

const instance: FulltextAttribution = {
    title,
    authors,
    year,
    publication,
    doi,
    license,
    license_statement,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
