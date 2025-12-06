# AnnotationsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**annotationAnalysesGet**](#annotationanalysesget) | **GET** /annotation-analyses/ | Get annotation analyses|
|[**annotationAnalysesIdGet**](#annotationanalysesidget) | **GET** /annotation-analyses/{id} | Your GET endpoint|
|[**annotationAnalysesIdPut**](#annotationanalysesidput) | **PUT** /annotation-analyses/{id} | Your PUT endpoint|
|[**annotationAnalysesPost**](#annotationanalysespost) | **POST** /annotation-analyses/ | Your POST endpoint|
|[**annotationsGet**](#annotationsget) | **GET** /annotations/ | Your GET endpoint|
|[**annotationsIdDelete**](#annotationsiddelete) | **DELETE** /annotations/{id} | DELETE an annotation|
|[**annotationsIdGet**](#annotationsidget) | **GET** /annotations/{id} | Your GET endpoint|
|[**annotationsIdPut**](#annotationsidput) | **PUT** /annotations/{id} | Update an annotation|
|[**annotationsPost**](#annotationspost) | **POST** /annotations/ | Post Annotation|

# **annotationAnalysesGet**
> NoteCollectionList annotationAnalysesGet()


### Example

```typescript
import {
    AnnotationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

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
    AnnotationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

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
    AnnotationsApi,
    Configuration,
    NoteCollectionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

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
    AnnotationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

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

# **annotationsGet**
> AnnotationList annotationsGet()

get annotations for an available studyset

### Example

```typescript
import {
    AnnotationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

let studysetId: string; //see all annotations connected to this studyset (optional) (default to undefined)
let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)

const { status, data } = await apiInstance.annotationsGet(
    studysetId,
    paginate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **studysetId** | [**string**] | see all annotations connected to this studyset | (optional) defaults to undefined|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|


### Return type

**AnnotationList**

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

# **annotationsIdDelete**
> annotationsIdDelete()

delete annotation

### Example

```typescript
import {
    AnnotationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.annotationsIdDelete(
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

# **annotationsIdGet**
> AnnotationReturn annotationsIdGet()

get an individual annotation

### Example

```typescript
import {
    AnnotationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

let id: string; // (default to undefined)
let _export: boolean; //return endpoint data in consumable/readable format (optional) (default to undefined)

const { status, data } = await apiInstance.annotationsIdGet(
    id,
    _export
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **_export** | [**boolean**] | return endpoint data in consumable/readable format | (optional) defaults to undefined|


### Return type

**AnnotationReturn**

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

# **annotationsIdPut**
> AnnotationReturn annotationsIdPut()

edit an existing annotation

### Example

```typescript
import {
    AnnotationsApi,
    Configuration,
    AnnotationRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

let id: string; // (default to undefined)
let annotationRequest: AnnotationRequest; // (optional)

const { status, data } = await apiInstance.annotationsIdPut(
    id,
    annotationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **annotationRequest** | **AnnotationRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AnnotationReturn**

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

# **annotationsPost**
> AnnotationReturn annotationsPost()

Create an annotation

### Example

```typescript
import {
    AnnotationsApi,
    Configuration,
    AnnotationRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new AnnotationsApi(configuration);

let source: 'neurostore' | 'neurovault' | 'pubmed' | 'neurosynth' | 'neuroquery' | 'pubget'; //the source of the resource you would like to filter/copy from (optional) (default to 'neurostore')
let sourceId: string; //id of the resource you are either filtering/copying on (optional) (default to undefined)
let annotationRequest: AnnotationRequest; // (optional)

const { status, data } = await apiInstance.annotationsPost(
    source,
    sourceId,
    annotationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **annotationRequest** | **AnnotationRequest**|  | |
| **source** | [**&#39;neurostore&#39; | &#39;neurovault&#39; | &#39;pubmed&#39; | &#39;neurosynth&#39; | &#39;neuroquery&#39; | &#39;pubget&#39;**]**Array<&#39;neurostore&#39; &#124; &#39;neurovault&#39; &#124; &#39;pubmed&#39; &#124; &#39;neurosynth&#39; &#124; &#39;neuroquery&#39; &#124; &#39;pubget&#39;>** | the source of the resource you would like to filter/copy from | (optional) defaults to 'neurostore'|
| **sourceId** | [**string**] | id of the resource you are either filtering/copying on | (optional) defaults to undefined|


### Return type

**AnnotationReturn**

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

