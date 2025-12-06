# AnalysesApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**analysesGet**](#analysesget) | **GET** /analyses/ | GET list of analyses|
|[**analysesIdDelete**](#analysesiddelete) | **DELETE** /analyses/{id} | DELETE an analysis|
|[**analysesIdGet**](#analysesidget) | **GET** /analyses/{id} | GET an analysis|
|[**analysesIdPut**](#analysesidput) | **PUT** /analyses/{id} | PUT/update an analysis|
|[**analysesPost**](#analysespost) | **POST** /analyses/ | POST/create an analysis|
|[**annotationAnalysesGet**](#annotationanalysesget) | **GET** /annotation-analyses/ | Get annotation analyses|
|[**annotationAnalysesIdGet**](#annotationanalysesidget) | **GET** /annotation-analyses/{id} | Your GET endpoint|
|[**annotationAnalysesIdPut**](#annotationanalysesidput) | **PUT** /annotation-analyses/{id} | Your PUT endpoint|
|[**annotationAnalysesPost**](#annotationanalysespost) | **POST** /annotation-analyses/ | Your POST endpoint|

# **analysesGet**
> AnalysisList analysesGet()

List all analyses performed across studies.

### Example

```typescript
import {
    AnalysesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let search: string; //search for entries that contain the substring (optional) (default to undefined)
let sort: string; //Parameter to sort results on (optional) (default to 'created_at')
let page: number; //page of results (optional) (default to undefined)
let desc: boolean; //sort results by descending order (as opposed to ascending order) (optional) (default to undefined)
let pageSize: number; //number of results to show on a page (optional) (default to undefined)
let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)
let study: string; //Filter tables by study id (optional) (default to undefined)
let name: string; //search the name field for a term (optional) (default to undefined)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)

const { status, data } = await apiInstance.analysesGet(
    search,
    sort,
    page,
    desc,
    pageSize,
    paginate,
    study,
    name,
    nested
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **search** | [**string**] | search for entries that contain the substring | (optional) defaults to undefined|
| **sort** | [**string**] | Parameter to sort results on | (optional) defaults to 'created_at'|
| **page** | [**number**] | page of results | (optional) defaults to undefined|
| **desc** | [**boolean**] | sort results by descending order (as opposed to ascending order) | (optional) defaults to undefined|
| **pageSize** | [**number**] | number of results to show on a page | (optional) defaults to undefined|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|
| **study** | [**string**] | Filter tables by study id | (optional) defaults to undefined|
| **name** | [**string**] | search the name field for a term | (optional) defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|


### Return type

**AnalysisList**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analysesIdDelete**
> analysesIdDelete()

delete an analysis

### Example

```typescript
import {
    AnalysesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.analysesIdDelete(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analysesIdGet**
> AnalysisReturn analysesIdGet()

Information pertaining to a particular analysis within a study.

### Example

```typescript
import {
    AnalysesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let id: string; // (default to undefined)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)

const { status, data } = await apiInstance.analysesIdGet(
    id,
    nested
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|


### Return type

**AnalysisReturn**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analysesIdPut**
> AnalysisReturn analysesIdPut()

Update an existing analysis.

### Example

```typescript
import {
    AnalysesApi,
    Configuration,
    AnalysisRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let id: string; // (default to undefined)
let analysisRequest: AnalysisRequest; // (optional)

const { status, data } = await apiInstance.analysesIdPut(
    id,
    analysisRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **analysisRequest** | **AnalysisRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AnalysisReturn**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**422** | Unprocessable Entity |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analysesPost**
> AnalysisReturn analysesPost()

create an analysis

### Example

```typescript
import {
    AnalysesApi,
    Configuration,
    AnalysisRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let analysisRequest: AnalysisRequest; // (optional)

const { status, data } = await apiInstance.analysesPost(
    analysisRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **analysisRequest** | **AnalysisRequest**|  | |


### Return type

**AnalysisReturn**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **annotationAnalysesGet**
> NoteCollectionList annotationAnalysesGet()


### Example

```typescript
import {
    AnalysesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)

const { status, data } = await apiInstance.annotationAnalysesGet(
    paginate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|


### Return type

**NoteCollectionList**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**2XX** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **annotationAnalysesIdGet**
> NoteCollectionReturn annotationAnalysesIdGet()


### Example

```typescript
import {
    AnalysesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.annotationAnalysesIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**NoteCollectionReturn**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **annotationAnalysesIdPut**
> NoteCollectionReturn annotationAnalysesIdPut()


### Example

```typescript
import {
    AnalysesApi,
    Configuration,
    NoteCollectionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let id: string; // (default to undefined)
let noteCollectionRequest: NoteCollectionRequest; // (optional)

const { status, data } = await apiInstance.annotationAnalysesIdPut(
    id,
    noteCollectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **noteCollectionRequest** | **NoteCollectionRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**NoteCollectionReturn**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **annotationAnalysesPost**
> Array<NoteCollectionReturn> annotationAnalysesPost()

This endpoint does not allow for creation, only modification of existing annotation-analyses. If you wish to create an annotation-analysis, post to the annotations endpoint and/or add the analysis to the appropriate study in the studyset, and the annotation-analysis will be created automatically. 

### Example

```typescript
import {
    AnalysesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalysesApi(configuration);

let noteCollectionRequest: Array<NoteCollectionRequest>; // (optional)

const { status, data } = await apiInstance.annotationAnalysesPost(
    noteCollectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **noteCollectionRequest** | **Array<NoteCollectionRequest>**|  | |


### Return type

**Array<NoteCollectionReturn>**

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

