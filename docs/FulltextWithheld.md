# FulltextWithheld

Why the text is not returned; null when it is.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reason** | **string** | &#x60;license&#x60;: the copy\&#39;s licence does not allow passing the text on. &#x60;access&#x60;: the copy was obtained under text-and-data-mining terms, or how it was obtained was not recorded. &#x60;no_copy_record&#x60;: nothing records the copy, so its licence is unknown. | [optional] [default to undefined]
**message** | **string** |  | [optional] [default to undefined]
**read_at** | **string** | Where a reader can get the paper (its DOI, else its PubMed Central page). | [optional] [default to undefined]

## Example

```typescript
import { FulltextWithheld } from './api';

const instance: FulltextWithheld = {
    reason,
    message,
    read_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
