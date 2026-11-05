# JournalReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** |  | [optional] [readonly] [default to undefined]
**openalex_id** | **string** | OpenAlex\&#39;s source id, bare (&#x60;S121666818&#x60;). | [optional] [default to undefined]
**title** | **string** | OpenAlex\&#39;s name for the source. | [optional] [default to undefined]
**abbreviation** | **string** | NLM\&#39;s ISO abbreviation, else its MEDLINE abbreviation. | [optional] [default to undefined]
**kind** | [**JournalKind**](JournalKind.md) |  | [optional] [default to undefined]
**issns** | **Array&lt;string&gt;** | Every ISSN of the title, print and electronic. | [optional] [default to undefined]
**issn_l** | **string** | Which of &#x60;issns&#x60; links the title\&#39;s print and electronic versions. | [optional] [default to undefined]
**nlm_id** | **string** | The NLM Catalog\&#39;s id for the title. | [optional] [default to undefined]
**wikidata_id** | **string** | Wikidata\&#39;s item for the title (&#x60;Q5936947&#x60;). | [optional] [default to undefined]

## Example

```typescript
import { JournalReturn } from './api';

const instance: JournalReturn = {
    created_at,
    updated_at,
    id,
    openalex_id,
    title,
    abbreviation,
    kind,
    issns,
    issn_l,
    nlm_id,
    wikidata_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
