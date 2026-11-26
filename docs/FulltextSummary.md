# FulltextSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** |  | [optional] [readonly] [default to undefined]
**base_study_id** | **string** |  | [optional] [default to undefined]
**source** | **string** | The ingestion source the text came from (&#x60;pubget&#x60;, &#x60;elsevier&#x60;, ...). | [optional] [default to undefined]
**source_version** | **string** |  | [optional] [default to undefined]
**license** | **string** | The licence of the copy the text was read from. | [optional] [default to undefined]
**sha256** | **string** |  | [optional] [default to undefined]
**text_copy** | **object** | The copy the text was read from (study_schema\&#39;s HeldCopy). | [optional] [default to undefined]
**preferred** | **boolean** | Whether this is the base study\&#39;s &#x60;fulltext_id&#x60;. | [optional] [default to undefined]
**redistributable** | **boolean** | Whether GET /fulltexts/{id} returns the text. | [optional] [default to undefined]
**attribution** | [**FulltextAttribution**](FulltextAttribution.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FulltextSummary } from './api';

const instance: FulltextSummary = {
    created_at,
    updated_at,
    id,
    base_study_id,
    source,
    source_version,
    license,
    sha256,
    text_copy,
    preferred,
    redistributable,
    attribution,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
