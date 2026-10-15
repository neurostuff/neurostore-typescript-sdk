# ReviewApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**neurostoreResourcesReviewReviewBundlesViewGet**](#neurostoreresourcesreviewreviewbundlesviewget) | **GET** /review/sources/{id}/bundle | Everything the review app needs to open one paper for the caller|
|[**neurostoreResourcesReviewReviewOpsViewPost**](#neurostoreresourcesreviewreviewopsviewpost) | **POST** /review/reviews/{id}/ops | Apply a batch of the owner\&#39;s ops to their review|
|[**neurostoreResourcesReviewReviewSourcesViewSearch**](#neurostoreresourcesreviewreviewsourcesviewsearch) | **GET** /review/sources/ | List papers loaded for review, with each reviewer\&#39;s progress|
|[**neurostoreResourcesReviewReviewsViewGet**](#neurostoreresourcesreviewreviewsviewget) | **GET** /review/reviews/{id} | One reviewer\&#39;s review of a paper|
|[**neurostoreResourcesReviewReviewsViewPatch**](#neurostoreresourcesreviewreviewsviewpatch) | **PATCH** /review/reviews/{id} | Submit, reopen, or mark as the reference review|
|[**neurostoreResourcesReviewSourceReviewsViewPut**](#neurostoreresourcesreviewsourcereviewsviewput) | **PUT** /review/sources/{id}/review | Start the caller\&#39;s review of a paper|

# **neurostoreResourcesReviewReviewBundlesViewGet**
> object neurostoreResourcesReviewReviewBundlesViewGet()


### Example

```typescript
import {
    ReviewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReviewApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.neurostoreResourcesReviewReviewBundlesViewGet(
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

# **neurostoreResourcesReviewReviewOpsViewPost**
> ReviewOpResult neurostoreResourcesReviewReviewOpsViewPost()

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

const { status, data } = await apiInstance.neurostoreResourcesReviewReviewOpsViewPost(
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
|**422** | Unprocessable Entity |  * X-Request-ID -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **neurostoreResourcesReviewReviewSourcesViewSearch**
> ReviewSourceList neurostoreResourcesReviewReviewSourcesViewSearch()


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

const { status, data } = await apiInstance.neurostoreResourcesReviewReviewSourcesViewSearch(
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

# **neurostoreResourcesReviewReviewsViewGet**
> ReviewDetail neurostoreResourcesReviewReviewsViewGet()

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

const { status, data } = await apiInstance.neurostoreResourcesReviewReviewsViewGet(
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

# **neurostoreResourcesReviewReviewsViewPatch**
> ReviewSummary neurostoreResourcesReviewReviewsViewPatch()

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

const { status, data } = await apiInstance.neurostoreResourcesReviewReviewsViewPatch(
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

# **neurostoreResourcesReviewSourceReviewsViewPut**
> ReviewSummary neurostoreResourcesReviewSourceReviewsViewPut()

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

const { status, data } = await apiInstance.neurostoreResourcesReviewSourceReviewsViewPut(
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

