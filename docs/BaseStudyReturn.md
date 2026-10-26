# BaseStudyReturn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | **object** |  | [optional] [default to undefined]
**versions** | [**Array&lt;BaseStudyVersionsInner&gt;**](BaseStudyVersionsInner.md) |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**publication** | **string** |  | [optional] [default to undefined]
**doi** | **string** |  | [optional] [default to undefined]
**pmid** | **string** |  | [optional] [default to undefined]
**authors** | **string** | The authors in published order. New values are joined with \&quot;; \&quot;, since a name may hold \&quot;, \&quot;; older values may be joined with \&quot;, \&quot; or \&quot;;\&quot;. When a paper\&#39;s structured author list has been uploaded the server derives this from it, and a value sent in a PUT, including null, is ignored. | [optional] [default to undefined]
**year** | **number** |  | [optional] [default to undefined]
**level** | **string** |  | [optional] [default to undefined]
**is_oa** | **boolean** |  | [optional] [default to undefined]
**pmcid** | **string** |  | [optional] [default to undefined]
**publication_status** | **string** | study_schema\&#39;s publication_status: &#x60;preprint&#x60; while only a preprint\&#39;s identifiers are known, &#x60;published&#x60; once a version of record\&#39;s are.  | [optional] [default to undefined]
**preprint_dois** | [**Array&lt;BaseStudyPreprintDoisInner&gt;**](BaseStudyPreprintDoisInner.md) | DOIs a preprint server registered for the paper, with the server. An identifier is held by one active base study: one another base study holds is not taken (see POST /base-studies). Returned normalized: DOIs in lower case.  | [optional] [default to undefined]
**preprint_pmids** | **Array&lt;string&gt;** | PubMed\&#39;s records of the paper\&#39;s preprint. | [optional] [default to undefined]
**preprint_pmcids** | **Array&lt;string&gt;** | PubMed Central\&#39;s copies of the paper\&#39;s preprint. | [optional] [default to undefined]
**alternative_dois** | **Array&lt;string&gt;** | Any other DOI of the paper that is neither the version of record\&#39;s &#x60;doi&#x60; nor a preprint\&#39;s.  | [optional] [default to undefined]
**alternative_pmids** | **Array&lt;string&gt;** | Any other PMID of the paper that is neither &#x60;pmid&#x60; nor a preprint\&#39;s. | [optional] [default to undefined]
**alternative_pmcids** | **Array&lt;string&gt;** | Any other PMCID of the paper that is neither &#x60;pmcid&#x60; nor a preprint\&#39;s. | [optional] [default to undefined]
**created_at** | **string** | time the resource was created on the database | [optional] [readonly] [default to undefined]
**updated_at** | **string** | when the resource was last modified/updated. | [optional] [readonly] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]
**user** | **string** | who owns the resource | [optional] [readonly] [default to undefined]
**username** | **string** | human readable username | [optional] [default to undefined]
**has_coordinates** | **boolean** |  | [optional] [default to undefined]
**has_images** | **boolean** |  | [optional] [default to undefined]
**has_z_maps** | **boolean** |  | [optional] [default to undefined]
**has_t_maps** | **boolean** |  | [optional] [default to undefined]
**has_beta_and_variance_maps** | **boolean** |  | [optional] [default to undefined]
**features** | **object** |  | [optional] [default to undefined]

## Example

```typescript
import { BaseStudyReturn } from './api';

const instance: BaseStudyReturn = {
    metadata,
    versions,
    name,
    description,
    publication,
    doi,
    pmid,
    authors,
    year,
    level,
    is_oa,
    pmcid,
    publication_status,
    preprint_dois,
    preprint_pmids,
    preprint_pmcids,
    alternative_dois,
    alternative_pmids,
    alternative_pmcids,
    created_at,
    updated_at,
    id,
    _public,
    user,
    username,
    has_coordinates,
    has_images,
    has_z_maps,
    has_t_maps,
    has_beta_and_variance_maps,
    features,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
