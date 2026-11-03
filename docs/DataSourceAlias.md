# DataSourceAlias


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [readonly] [default to undefined]
**alias** | **string** |  | [default to undefined]
**tier** | **string** | What a match on the alias needs: &#x60;name&#x60;, a full name matched case-insensitively; &#x60;safe&#x60;, an acronym that stands alone; &#x60;context&#x60;, an acronym needing a dataset or imaging word nearby; &#x60;defined&#x60;, an acronym needing one of the data source\&#39;s names in the same paper; &#x60;qualified&#x60;, a common word needing a qualifier such as \&quot;dataset\&quot; or an accession. | [default to undefined]

## Example

```typescript
import { DataSourceAlias } from './api';

const instance: DataSourceAlias = {
    id,
    alias,
    tier,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
