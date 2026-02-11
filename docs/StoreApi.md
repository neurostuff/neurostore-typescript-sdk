# StoreApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**studiesGet**](#studiesget) | **GET** /studies/ | GET a list of studies|
|[**studiesIdDelete**](#studiesiddelete) | **DELETE** /studies/{id} | DELETE a study|
|[**studiesIdGet**](#studiesidget) | **GET** /studies/{id} | GET a study|
|[**studiesIdPut**](#studiesidput) | **PUT** /studies/{id} | PUT/update a study|
|[**studiesPost**](#studiespost) | **POST** /studies/ | POST/create a study|
|[**studysetsIdDelete**](#studysetsiddelete) | **DELETE** /studysets/{id} | DELETE a studyset|
|[**studysetsIdGet**](#studysetsidget) | **GET** /studysets/{id} | GET a studyset|
|[**studysetsIdPut**](#studysetsidput) | **PUT** /studysets/{id} | PUT/update a studyset|
|[**studysetsPost**](#studysetspost) | **POST** /studysets/ | POST/create a studyset|

# **studiesGet**
> StudyList studiesGet()

List studies

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let search: string; //search for entries that contain the substring (optional) (default to undefined)
let sort: string; //Parameter to sort results on (optional) (default to 'created_at')
let page: number; //page of results (optional) (default to undefined)
let desc: boolean; //sort results by descending order (as opposed to ascending order) (optional) (default to undefined)
let pageSize: number; //number of results to show on a page (optional) (default to undefined)
let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)
let name: string; //search the name field for a term (optional) (default to undefined)
let description: string; //search description field for a term (optional) (default to undefined)
let sourceId: string; //id of the resource you are either filtering/copying on (optional) (default to undefined)
let unique: any; //whether to list clones with originals (optional) (default to undefined)
let source: 'neurostore' | 'neurovault' | 'pubmed' | 'neurosynth' | 'neuroquery' | 'pubget'; //the source of the resource you would like to filter/copy from (optional) (default to 'neurostore')
let authors: string; //search authors (optional) (default to undefined)
let userId: string; //user id you want to filter by (optional) (default to undefined)
let dataType: 'coordinate' | 'image' | 'both'; //whether searching for studies that contain coordinates, images, or both (optional) (default to undefined)
let mapType: 'z' | 't' | 'beta_variance' | 'any'; //filter by stored map-type flags (optional) (default to undefined)
let studysetOwner: string; //for all studies filter which studysets are listed based on who owns the studyset (optional) (default to undefined)
let level: 'group' | 'meta'; //select between studies with group results or meta results (optional) (default to 'group')
let pmid: string; //search for particular pmid (optional) (default to undefined)
let doi: string; //search for study with specific doi (optional) (default to undefined)
let flat: boolean; //do not return any embedded relationships. When set, it is incompatible with nested.  (optional) (default to undefined)

const { status, data } = await apiInstance.studiesGet(
    search,
    sort,
    page,
    desc,
    pageSize,
    paginate,
    nested,
    name,
    description,
    sourceId,
    unique,
    source,
    authors,
    userId,
    dataType,
    mapType,
    studysetOwner,
    level,
    pmid,
    doi,
    flat
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
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|
| **name** | [**string**] | search the name field for a term | (optional) defaults to undefined|
| **description** | [**string**] | search description field for a term | (optional) defaults to undefined|
| **sourceId** | [**string**] | id of the resource you are either filtering/copying on | (optional) defaults to undefined|
| **unique** | **any** | whether to list clones with originals | (optional) defaults to undefined|
| **source** | [**&#39;neurostore&#39; | &#39;neurovault&#39; | &#39;pubmed&#39; | &#39;neurosynth&#39; | &#39;neuroquery&#39; | &#39;pubget&#39;**]**Array<&#39;neurostore&#39; &#124; &#39;neurovault&#39; &#124; &#39;pubmed&#39; &#124; &#39;neurosynth&#39; &#124; &#39;neuroquery&#39; &#124; &#39;pubget&#39;>** | the source of the resource you would like to filter/copy from | (optional) defaults to 'neurostore'|
| **authors** | [**string**] | search authors | (optional) defaults to undefined|
| **userId** | [**string**] | user id you want to filter by | (optional) defaults to undefined|
| **dataType** | [**&#39;coordinate&#39; | &#39;image&#39; | &#39;both&#39;**]**Array<&#39;coordinate&#39; &#124; &#39;image&#39; &#124; &#39;both&#39;>** | whether searching for studies that contain coordinates, images, or both | (optional) defaults to undefined|
| **mapType** | [**&#39;z&#39; | &#39;t&#39; | &#39;beta_variance&#39; | &#39;any&#39;**]**Array<&#39;z&#39; &#124; &#39;t&#39; &#124; &#39;beta_variance&#39; &#124; &#39;any&#39;>** | filter by stored map-type flags | (optional) defaults to undefined|
| **studysetOwner** | [**string**] | for all studies filter which studysets are listed based on who owns the studyset | (optional) defaults to undefined|
| **level** | [**&#39;group&#39; | &#39;meta&#39;**]**Array<&#39;group&#39; &#124; &#39;meta&#39;>** | select between studies with group results or meta results | (optional) defaults to 'group'|
| **pmid** | [**string**] | search for particular pmid | (optional) defaults to undefined|
| **doi** | [**string**] | search for study with specific doi | (optional) defaults to undefined|
| **flat** | [**boolean**] | do not return any embedded relationships. When set, it is incompatible with nested.  | (optional) defaults to undefined|


### Return type

**StudyList**

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

# **studiesIdDelete**
> studiesIdDelete()

delete a study

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.studiesIdDelete(
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

# **studiesIdGet**
> StudyReturn studiesIdGet()

Get a study.

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)
let studysetOwner: string; //for all studies filter which studysets are listed based on who owns the studyset (optional) (default to undefined)
let flat: boolean; //do not return any embedded relationships. When set, it is incompatible with nested.  (optional) (default to undefined)

const { status, data } = await apiInstance.studiesIdGet(
    id,
    nested,
    studysetOwner,
    flat
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|
| **studysetOwner** | [**string**] | for all studies filter which studysets are listed based on who owns the studyset | (optional) defaults to undefined|
| **flat** | [**boolean**] | do not return any embedded relationships. When set, it is incompatible with nested.  | (optional) defaults to undefined|


### Return type

**StudyReturn**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Study Found |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **studiesIdPut**
> StudyReturn studiesIdPut()

Update a study.

### Example

```typescript
import {
    StoreApi,
    Configuration,
    StudyRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let studyRequest: StudyRequest; // (optional)

const { status, data } = await apiInstance.studiesIdPut(
    id,
    studyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **studyRequest** | **StudyRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**StudyReturn**

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

# **studiesPost**
> StudyReturn studiesPost()

Create a study

### Example

```typescript
import {
    StoreApi,
    Configuration,
    StudyRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let source: 'neurostore' | 'neurovault' | 'pubmed' | 'neurosynth' | 'neuroquery' | 'pubget'; //the source of the resource you would like to filter/copy from (optional) (default to 'neurostore')
let sourceId: string; //id of the resource you are either filtering/copying on (optional) (default to undefined)
let studyRequest: StudyRequest; // (optional)

const { status, data } = await apiInstance.studiesPost(
    source,
    sourceId,
    studyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **studyRequest** | **StudyRequest**|  | |
| **source** | [**&#39;neurostore&#39; | &#39;neurovault&#39; | &#39;pubmed&#39; | &#39;neurosynth&#39; | &#39;neuroquery&#39; | &#39;pubget&#39;**]**Array<&#39;neurostore&#39; &#124; &#39;neurovault&#39; &#124; &#39;pubmed&#39; &#124; &#39;neurosynth&#39; &#124; &#39;neuroquery&#39; &#124; &#39;pubget&#39;>** | the source of the resource you would like to filter/copy from | (optional) defaults to 'neurostore'|
| **sourceId** | [**string**] | id of the resource you are either filtering/copying on | (optional) defaults to undefined|


### Return type

**StudyReturn**

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

# **studysetsIdDelete**
> studysetsIdDelete()

delete a studyset

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.studysetsIdDelete(
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

# **studysetsIdGet**
> StudysetReturn studysetsIdGet()

Retrieve the information of a studyset with the matching studyset ID.

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)
let summary: boolean; //return a lightweight summary payload with study metadata and per-analysis coordinate counts; incompatible with nested (optional) (default to undefined)
let gzip: boolean; //return the content as gzipped content (optional) (default to undefined)

const { status, data } = await apiInstance.studysetsIdGet(
    id,
    nested,
    summary,
    gzip
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|
| **summary** | [**boolean**] | return a lightweight summary payload with study metadata and per-analysis coordinate counts; incompatible with nested | (optional) defaults to undefined|
| **gzip** | [**boolean**] | return the content as gzipped content | (optional) defaults to undefined|


### Return type

**StudysetReturn**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/gzip


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | studyset found |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **studysetsIdPut**
> StudysetReturn studysetsIdPut()

Update a studyset.

### Example

```typescript
import {
    StoreApi,
    Configuration,
    StudysetRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let studysetRequest: StudysetRequest; // (optional)

const { status, data } = await apiInstance.studysetsIdPut(
    id,
    studysetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **studysetRequest** | **StudysetRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**StudysetReturn**

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

# **studysetsPost**
> StudysetReturn studysetsPost()

Create a studyset. When `source_id` is provided, Neurostore clones an existing studyset owned by any user into a new studyset owned by the caller, copying studies and (by default) annotations.

### Example

```typescript
import {
    StoreApi,
    Configuration,
    StudysetRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let sourceId: string; //id of the resource you are either filtering/copying on (optional) (default to undefined)
let source: 'neurostore' | 'neurovault' | 'pubmed' | 'neurosynth' | 'neuroquery' | 'pubget'; //the source of the resource you would like to filter/copy from (optional) (default to 'neurostore')
let copyAnnotations: boolean; //When cloning a studyset, copy annotations and their notes when true (default). (optional) (default to true)
let studysetRequest: StudysetRequest; // (optional)

const { status, data } = await apiInstance.studysetsPost(
    sourceId,
    source,
    copyAnnotations,
    studysetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **studysetRequest** | **StudysetRequest**|  | |
| **sourceId** | [**string**] | id of the resource you are either filtering/copying on | (optional) defaults to undefined|
| **source** | [**&#39;neurostore&#39; | &#39;neurovault&#39; | &#39;pubmed&#39; | &#39;neurosynth&#39; | &#39;neuroquery&#39; | &#39;pubget&#39;**]**Array<&#39;neurostore&#39; &#124; &#39;neurovault&#39; &#124; &#39;pubmed&#39; &#124; &#39;neurosynth&#39; &#124; &#39;neuroquery&#39; &#124; &#39;pubget&#39;>** | the source of the resource you would like to filter/copy from | (optional) defaults to 'neurostore'|
| **copyAnnotations** | [**boolean**] | When cloning a studyset, copy annotations and their notes when true (default). | (optional) defaults to true|


### Return type

**StudysetReturn**

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

