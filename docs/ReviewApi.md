# ReviewApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**reviewExportsPost**](#reviewexportspost) | **POST** /review/exports/ | Export the reviews that match the filters as a zip of layout trees|
|[**reviewImportsPost**](#reviewimportspost) | **POST** /review/imports/ | Load the papers of a study_schema layout zip for review|
|[**reviewReviewsIdExportGet**](#reviewreviewsidexportget) | **GET** /review/reviews/{id}/export | Export one review as a study_schema layout zip|
|[**reviewReviewsIdGet**](#reviewreviewsidget) | **GET** /review/reviews/{id} | One reviewer\&#39;s review of a paper|
|[**reviewReviewsIdOpsPost**](#reviewreviewsidopspost) | **POST** /review/reviews/{id}/ops | Apply a batch of the owner\&#39;s ops to their review|
|[**reviewReviewsIdPatch**](#reviewreviewsidpatch) | **PATCH** /review/reviews/{id} | Submit, reopen, or mark as the reference review|
|[**reviewSourcesGet**](#reviewsourcesget) | **GET** /review/sources/ | List papers loaded for review, with each reviewer\&#39;s progress|
|[**reviewSourcesIdBundleGet**](#reviewsourcesidbundleget) | **GET** /review/sources/{id}/bundle | Everything the review app needs to open one paper for the caller|
|[**reviewSourcesIdReviewPut**](#reviewsourcesidreviewput) | **PUT** /review/sources/{id}/review | Start the caller\&#39;s review of a paper|

# **reviewExportsPost**
> File reviewExportsPost()

One layout tree per reviewer, under the reviewer\'s id. A source with no review is included, as loaded under _source/, only when include_unreviewed is true. An empty filter list means no filter. include_unreviewed cannot be combined with user_ids or states; that request is refused with 422. The whole zip is built in memory before the response is sent, so split a large export with source_ids or base_study_ids. 

### Example

```typescript
import {
    ReviewApi,
    Configuration,
    ReviewExportsPostRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let reviewExportsPostRequest: ReviewExportsPostRequest; // (optional)

const { status, data } = await apiInstance.reviewExportsPost(
    reviewExportsPostRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **reviewExportsPostRequest** | **ReviewExportsPostRequest**|  | |


### Return type

**File**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/zip


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A zip of the layout trees |  * Content-Disposition - An attachment named review-exports.zip <br>  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**422** | include_unreviewed was combined with a reviewer or state filter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewImportsPost**
> ReviewImportReport reviewImportsPost()

Lead reviewers only (admin-reviewer and admin). Each paper is checked and stored on its own: the report names what loaded, what was already loaded and what failed, and why. A file that is not a layout is refused whole. 

### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let file: File; //A zip of a study_schema layout, at most 200 MB. (default to undefined)

const { status, data } = await apiInstance.reviewImportsPost(
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **file** | [**File**] | A zip of a study_schema layout, at most 200 MB. | defaults to undefined|


### Return type

**ReviewImportReport**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The report of what each paper did |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**413** | The file is over 200 MB |  * X-Request-ID -  <br>  |
|**422** | Unprocessable Entity |  * X-Request-ID -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewReviewsIdExportGet**
> File reviewReviewsIdExportGet()

Any reviewer may export any review. The zip holds the paper\'s documents and text, the review\'s record, its coordinate revision when it has one, and its ops in seq order. The record is never changed by the export; run/provenance/<id>.json beside it names the review, its state and the source record it derives from. The whole zip is built in memory before the response is sent. 

### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.reviewReviewsIdExportGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**File**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/zip, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A zip of the review\&#39;s layout |  * Content-Disposition - An attachment named review-exports.zip <br>  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  * X-Request-ID -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewReviewsIdGet**
> ReviewDetail reviewReviewsIdGet()

Any reviewer may read any review.

### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.reviewReviewsIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ReviewDetail**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  * X-Request-ID -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewReviewsIdOpsPost**
> ReviewOpResult reviewReviewsIdOpsPost()

Only the review\'s owner. The batch applies whole or not at all. A batch whose every client_op_id is already stored is a replay: it returns the stored ops and applies nothing. 

### Example

```typescript
import {
    ReviewApi,
    Configuration,
    ReviewOpBatch
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)
let reviewOpBatch: ReviewOpBatch; // (optional)

const { status, data } = await apiInstance.reviewReviewsIdOpsPost(
    id,
    reviewOpBatch
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **reviewOpBatch** | **ReviewOpBatch**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ReviewOpResult**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The ops applied, or the stored ops of a replay |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  * X-Request-ID -  <br>  |
|**409** | The review is not in_progress, expected_last_seq is not the review\&#39;s last_seq (the body carries last_seq), or only some of the batch\&#39;s client_op_ids are stored  |  -  |
|**422** | The batch does not validate, an op cannot be applied, or the record would fail study_schema. Each refused op is one error: field ops/&lt;index&gt;, code REJECTED, and context with op_index (an integer) and client_op_id. The message names the problem. A problem with the batch as a whole has field ops and no op index. Nothing is applied.  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewReviewsIdPatch**
> ReviewSummary reviewReviewsIdPatch()

The owner moves in_progress to submitted and back. Only an admin sets reference, and a paper has at most one reference review. 

### Example

```typescript
import {
    ReviewApi,
    Configuration,
    ReviewStatePatch
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)
let reviewStatePatch: ReviewStatePatch; // (optional)

const { status, data } = await apiInstance.reviewReviewsIdPatch(
    id,
    reviewStatePatch
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **reviewStatePatch** | **ReviewStatePatch**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ReviewSummary**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  * X-Request-ID -  <br>  |
|**409** | The transition is not allowed, or the paper already has a reference review |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewSourcesGet**
> ReviewSourceList reviewSourcesGet()


### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let page: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let baseStudyId: string; //Only the sources of this base study. (optional) (default to undefined)
let mine: boolean; //Only the sources the caller has a review of. (optional) (default to false)

const { status, data } = await apiInstance.reviewSourcesGet(
    page,
    pageSize,
    baseStudyId,
    mine
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **baseStudyId** | [**string**] | Only the sources of this base study. | (optional) defaults to undefined|
| **mine** | [**boolean**] | Only the sources the caller has a review of. | (optional) defaults to false|


### Return type

**ReviewSourceList**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewSourcesIdBundleGet**
> object reviewSourcesIdBundleGet()


### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.reviewSourcesIdBundleGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**object**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  * X-Request-ID -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reviewSourcesIdReviewPut**
> ReviewSummary reviewSourcesIdReviewPut()

Starts the caller\'s review, in_progress, from the source\'s extraction record. A repeat call returns the existing review. 

### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.reviewSourcesIdReviewPut(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ReviewSummary**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The caller\&#39;s review already existed |  -  |
|**201** | The caller\&#39;s review was started |  -  |
|**401** | Unauthorized |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  * X-Request-ID -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

