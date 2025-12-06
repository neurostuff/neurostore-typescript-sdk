# StoreApi

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
|[**annotationsGet**](#annotationsget) | **GET** /annotations/ | Your GET endpoint|
|[**annotationsIdDelete**](#annotationsiddelete) | **DELETE** /annotations/{id} | DELETE an annotation|
|[**annotationsIdGet**](#annotationsidget) | **GET** /annotations/{id} | Your GET endpoint|
|[**annotationsIdPut**](#annotationsidput) | **PUT** /annotations/{id} | Update an annotation|
|[**annotationsPost**](#annotationspost) | **POST** /annotations/ | Post Annotation|
|[**baseStudiesGet**](#basestudiesget) | **GET** /base-studies/ | |
|[**baseStudiesIdGet**](#basestudiesidget) | **GET** /base-studies/{id} | Your GET endpoint|
|[**baseStudiesIdPut**](#basestudiesidput) | **PUT** /base-studies/{id} | |
|[**baseStudiesPost**](#basestudiespost) | **POST** /base-studies/ | |
|[**conditionsGet**](#conditionsget) | **GET** /conditions/ | GET Conditions|
|[**conditionsIdDelete**](#conditionsiddelete) | **DELETE** /conditions/{id} | DELETE a condition|
|[**conditionsIdGet**](#conditionsidget) | **GET** /conditions/{id} | GET a condition|
|[**conditionsIdPut**](#conditionsidput) | **PUT** /conditions/{id} | PUT/update a condition|
|[**conditionsPost**](#conditionspost) | **POST** /conditions/ | POST/Create a condition|
|[**imagesGet**](#imagesget) | **GET** /images/ | GET a list of images|
|[**imagesIdDelete**](#imagesiddelete) | **DELETE** /images/{id} | DELETE an image|
|[**imagesIdGet**](#imagesidget) | **GET** /images/{id} | GET an image|
|[**imagesIdPut**](#imagesidput) | **PUT** /images/{id} | PUT/update an image|
|[**imagesPost**](#imagespost) | **POST** /images/ | POST/create an image|
|[**pointsGet**](#pointsget) | **GET** /points/ | Get Points|
|[**pointsIdDelete**](#pointsiddelete) | **DELETE** /points/{id} | DELETE a point|
|[**pointsIdGet**](#pointsidget) | **GET** /points/{id} | GET a point|
|[**pointsIdPut**](#pointsidput) | **PUT** /points/{id} | PUT/update a point|
|[**pointsPost**](#pointspost) | **POST** /points/ | POST Points|
|[**studiesGet**](#studiesget) | **GET** /studies/ | GET a list of studies|
|[**studiesIdDelete**](#studiesiddelete) | **DELETE** /studies/{id} | DELETE a study|
|[**studiesIdGet**](#studiesidget) | **GET** /studies/{id} | GET a study|
|[**studiesIdPut**](#studiesidput) | **PUT** /studies/{id} | PUT/update a study|
|[**studiesPost**](#studiespost) | **POST** /studies/ | POST/create a study|
|[**studysetsIdDelete**](#studysetsiddelete) | **DELETE** /studysets/{id} | DELETE a studyset|
|[**studysetsIdGet**](#studysetsidget) | **GET** /studysets/{id} | GET a studyset|
|[**studysetsIdPut**](#studysetsidput) | **PUT** /studysets/{id} | PUT/update a studyset|
|[**studysetsPost**](#studysetspost) | **POST** /studysets/ | POST/create a studyset|
|[**tablesGet**](#tablesget) | **GET** /tables/ | GET list of tables|
|[**tablesIdDelete**](#tablesiddelete) | **DELETE** /tables/{id} | DELETE a table|
|[**tablesIdGet**](#tablesidget) | **GET** /tables/{id} | GET a table|
|[**tablesIdPut**](#tablesidput) | **PUT** /tables/{id} | PUT/update a table|
|[**tablesPost**](#tablespost) | **POST** /tables/ | POST/create a table|

# **analysesGet**
> AnalysisList analysesGet()

List all analyses performed across studies.

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration,
    AnalysisRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration,
    AnalysisRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration,
    NoteCollectionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration,
    AnnotationRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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
    StoreApi,
    Configuration,
    AnnotationRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

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

# **baseStudiesGet**
> BaseStudyList baseStudiesGet()


### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)
let yearMin: number; //Minimum publication year (inclusive) for study search (optional) (default to undefined)
let x: number; //X coordinate for spatial query (requires y, z, and radius) (optional) (default to undefined)
let y: number; //Y coordinate for spatial query (requires x, z, and radius) (optional) (default to undefined)
let z: number; //Z coordinate for spatial query (requires x, y, and radius) (optional) (default to undefined)
let radius: number; //Radius for spatial query (requires x, y, and z) (optional) (default to undefined)
let yearMax: number; //Maximum publication year (inclusive) for study search (optional) (default to undefined)
let featureFilter: Array<string>; //Filter studies by feature content. Format: \"PipelineName[:version]:field_path=value\". Examples:   - \"TestPipeline:1.0.0:predictions.age_mean>20\" (specific version)   - \"TestPipeline:groups.diagnosis=ADHD\" (latest version)  Field path supports array notation with [], regex search with ~, and comparisons with =, >, <, >=, <=.  (optional) (default to undefined)
let pipelineConfig: Array<string>; //Filter studies by pipeline config content. Format: \"PipelineName[:version]:config_path=value\". Examples:   - \"TestPipeline:1.0.0:settings.min_age=20\" (specific version)   - \"TestPipeline:model.type=linear\" (latest version)  Config path supports array notation with [], regex search with ~, and comparisons with =, >, <, >=, <=.  (optional) (default to undefined)
let featureDisplay: string; //display features from pipelines (optional) (default to undefined)
let semanticSearch: string; //Semantic search query string (optional) (default to undefined)
let pipelineConfigId: string; //Pipeline configuration identifier to filter studies (optional) (default to undefined)
let distanceThreshold: number; //Distance threshold for semantic search (default 0.5) (optional) (default to undefined)
let overallCap: number; //Maximum number of overall results to return (default 3000) (optional) (default to undefined)
let featureFlatten: boolean; // (optional) (default to undefined)
let search: string; //search for entries that contain the substring (optional) (default to undefined)
let sort: string; //Parameter to sort results on (optional) (default to 'created_at')
let page: number; //page of results (optional) (default to undefined)
let desc: boolean; //sort results by descending order (as opposed to ascending order) (optional) (default to undefined)
let pageSize: number; //number of results to show on a page (optional) (default to undefined)
let name: string; //search the name field for a term (optional) (default to undefined)
let description: string; //search description field for a term (optional) (default to undefined)
let authors: string; //search authors (optional) (default to undefined)
let level: 'group' | 'meta'; //select between studies with group results or meta results (optional) (default to 'group')
let dataType: 'coordinate' | 'image' | 'both'; //whether searching for studies that contain coordinates, images, or both (optional) (default to undefined)
let isOa: boolean; // (optional) (default to undefined)
let publication: string; //search for papers from a particular journal (optional) (default to undefined)
let pmid: string; //search for particular pmid (optional) (default to undefined)
let doi: string; //search for study with specific doi (optional) (default to undefined)
let flat: boolean; //do not return any embedded relationships. When set, it is incompatible with nested.  (optional) (default to undefined)
let info: boolean; //show additional for endpoint-object relationships without being fully nested. Incompatible with nested (optional) (default to undefined)
let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)

const { status, data } = await apiInstance.baseStudiesGet(
    nested,
    yearMin,
    x,
    y,
    z,
    radius,
    yearMax,
    featureFilter,
    pipelineConfig,
    featureDisplay,
    semanticSearch,
    pipelineConfigId,
    distanceThreshold,
    overallCap,
    featureFlatten,
    search,
    sort,
    page,
    desc,
    pageSize,
    name,
    description,
    authors,
    level,
    dataType,
    isOa,
    publication,
    pmid,
    doi,
    flat,
    info,
    paginate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|
| **yearMin** | [**number**] | Minimum publication year (inclusive) for study search | (optional) defaults to undefined|
| **x** | [**number**] | X coordinate for spatial query (requires y, z, and radius) | (optional) defaults to undefined|
| **y** | [**number**] | Y coordinate for spatial query (requires x, z, and radius) | (optional) defaults to undefined|
| **z** | [**number**] | Z coordinate for spatial query (requires x, y, and radius) | (optional) defaults to undefined|
| **radius** | [**number**] | Radius for spatial query (requires x, y, and z) | (optional) defaults to undefined|
| **yearMax** | [**number**] | Maximum publication year (inclusive) for study search | (optional) defaults to undefined|
| **featureFilter** | **Array&lt;string&gt;** | Filter studies by feature content. Format: \&quot;PipelineName[:version]:field_path&#x3D;value\&quot;. Examples:   - \&quot;TestPipeline:1.0.0:predictions.age_mean&gt;20\&quot; (specific version)   - \&quot;TestPipeline:groups.diagnosis&#x3D;ADHD\&quot; (latest version)  Field path supports array notation with [], regex search with ~, and comparisons with &#x3D;, &gt;, &lt;, &gt;&#x3D;, &lt;&#x3D;.  | (optional) defaults to undefined|
| **pipelineConfig** | **Array&lt;string&gt;** | Filter studies by pipeline config content. Format: \&quot;PipelineName[:version]:config_path&#x3D;value\&quot;. Examples:   - \&quot;TestPipeline:1.0.0:settings.min_age&#x3D;20\&quot; (specific version)   - \&quot;TestPipeline:model.type&#x3D;linear\&quot; (latest version)  Config path supports array notation with [], regex search with ~, and comparisons with &#x3D;, &gt;, &lt;, &gt;&#x3D;, &lt;&#x3D;.  | (optional) defaults to undefined|
| **featureDisplay** | [**string**] | display features from pipelines | (optional) defaults to undefined|
| **semanticSearch** | [**string**] | Semantic search query string | (optional) defaults to undefined|
| **pipelineConfigId** | [**string**] | Pipeline configuration identifier to filter studies | (optional) defaults to undefined|
| **distanceThreshold** | [**number**] | Distance threshold for semantic search (default 0.5) | (optional) defaults to undefined|
| **overallCap** | [**number**] | Maximum number of overall results to return (default 3000) | (optional) defaults to undefined|
| **featureFlatten** | [**boolean**] |  | (optional) defaults to undefined|
| **search** | [**string**] | search for entries that contain the substring | (optional) defaults to undefined|
| **sort** | [**string**] | Parameter to sort results on | (optional) defaults to 'created_at'|
| **page** | [**number**] | page of results | (optional) defaults to undefined|
| **desc** | [**boolean**] | sort results by descending order (as opposed to ascending order) | (optional) defaults to undefined|
| **pageSize** | [**number**] | number of results to show on a page | (optional) defaults to undefined|
| **name** | [**string**] | search the name field for a term | (optional) defaults to undefined|
| **description** | [**string**] | search description field for a term | (optional) defaults to undefined|
| **authors** | [**string**] | search authors | (optional) defaults to undefined|
| **level** | [**&#39;group&#39; | &#39;meta&#39;**]**Array<&#39;group&#39; &#124; &#39;meta&#39;>** | select between studies with group results or meta results | (optional) defaults to 'group'|
| **dataType** | [**&#39;coordinate&#39; | &#39;image&#39; | &#39;both&#39;**]**Array<&#39;coordinate&#39; &#124; &#39;image&#39; &#124; &#39;both&#39;>** | whether searching for studies that contain coordinates, images, or both | (optional) defaults to undefined|
| **isOa** | [**boolean**] |  | (optional) defaults to undefined|
| **publication** | [**string**] | search for papers from a particular journal | (optional) defaults to undefined|
| **pmid** | [**string**] | search for particular pmid | (optional) defaults to undefined|
| **doi** | [**string**] | search for study with specific doi | (optional) defaults to undefined|
| **flat** | [**boolean**] | do not return any embedded relationships. When set, it is incompatible with nested.  | (optional) defaults to undefined|
| **info** | [**boolean**] | show additional for endpoint-object relationships without being fully nested. Incompatible with nested | (optional) defaults to undefined|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|


### Return type

**BaseStudyList**

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

# **baseStudiesIdGet**
> BaseStudyReturn baseStudiesIdGet()


### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let flat: boolean; //do not return any embedded relationships. When set, it is incompatible with nested.  (optional) (default to undefined)
let info: boolean; //show additional for endpoint-object relationships without being fully nested. Incompatible with nested (optional) (default to undefined)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)

const { status, data } = await apiInstance.baseStudiesIdGet(
    id,
    flat,
    info,
    nested
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **flat** | [**boolean**] | do not return any embedded relationships. When set, it is incompatible with nested.  | (optional) defaults to undefined|
| **info** | [**boolean**] | show additional for endpoint-object relationships without being fully nested. Incompatible with nested | (optional) defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|


### Return type

**BaseStudyReturn**

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

# **baseStudiesIdPut**
> BaseStudyReturn baseStudiesIdPut()


### Example

```typescript
import {
    StoreApi,
    Configuration,
    BaseStudy
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let baseStudy: BaseStudy; // (optional)

const { status, data } = await apiInstance.baseStudiesIdPut(
    id,
    baseStudy
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **baseStudy** | **BaseStudy**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**BaseStudyReturn**

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

# **baseStudiesPost**
> BaseStudiesPost200Response baseStudiesPost()


### Example

```typescript
import {
    StoreApi,
    Configuration,
    BaseStudiesPostRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let baseStudiesPostRequest: BaseStudiesPostRequest; // (optional)

const { status, data } = await apiInstance.baseStudiesPost(
    baseStudiesPostRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **baseStudiesPostRequest** | **BaseStudiesPostRequest**|  | |


### Return type

**BaseStudiesPost200Response**

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

# **conditionsGet**
> ConditionList conditionsGet()

Get all conditions

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
let name: string; //search the name field for a term (optional) (default to undefined)
let description: string; //search description field for a term (optional) (default to undefined)

const { status, data } = await apiInstance.conditionsGet(
    search,
    sort,
    page,
    desc,
    pageSize,
    paginate,
    name,
    description
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
| **name** | [**string**] | search the name field for a term | (optional) defaults to undefined|
| **description** | [**string**] | search description field for a term | (optional) defaults to undefined|


### Return type

**ConditionList**

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

# **conditionsIdDelete**
> conditionsIdDelete()

delete a condition

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.conditionsIdDelete(
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

# **conditionsIdGet**
> ConditionReturn conditionsIdGet()

Retrieve a condition (e.g., 2-back) that can be used in contrasts (e.g., 2-back - 1-back)

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.conditionsIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ConditionReturn**

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

# **conditionsIdPut**
> ConditionReturn conditionsIdPut()

update a condition

### Example

```typescript
import {
    StoreApi,
    Configuration,
    ConditionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let conditionRequest: ConditionRequest; // (optional)

const { status, data } = await apiInstance.conditionsIdPut(
    id,
    conditionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conditionRequest** | **ConditionRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ConditionReturn**

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

# **conditionsPost**
> ConditionReturn conditionsPost()

Create a condition

### Example

```typescript
import {
    StoreApi,
    Configuration,
    ConditionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let conditionRequest: ConditionRequest; // (optional)

const { status, data } = await apiInstance.conditionsPost(
    conditionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conditionRequest** | **ConditionRequest**|  | |


### Return type

**ConditionReturn**

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

# **imagesGet**
> ImageList imagesGet()

Retrieve and list images.

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
let filename: string; //search filename field (optional) (default to undefined)
let analysisName: string; //search analysis_name field (optional) (default to undefined)
let valueType: string; //search value_type field (optional) (default to undefined)
let space: string; //search space field (optional) (default to undefined)

const { status, data } = await apiInstance.imagesGet(
    search,
    sort,
    page,
    desc,
    pageSize,
    paginate,
    filename,
    analysisName,
    valueType,
    space
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
| **filename** | [**string**] | search filename field | (optional) defaults to undefined|
| **analysisName** | [**string**] | search analysis_name field | (optional) defaults to undefined|
| **valueType** | [**string**] | search value_type field | (optional) defaults to undefined|
| **space** | [**string**] | search space field | (optional) defaults to undefined|


### Return type

**ImageList**

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

# **imagesIdDelete**
> imagesIdDelete()

delete an image

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.imagesIdDelete(
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

# **imagesIdGet**
> ImageReturn imagesIdGet()

Retrieve information about a particular image from an analysis.

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.imagesIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ImageReturn**

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

# **imagesIdPut**
> ImageReturn imagesIdPut()

Update a specific image.

### Example

```typescript
import {
    StoreApi,
    Configuration,
    ImageRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let imageRequest: ImageRequest; // (optional)

const { status, data } = await apiInstance.imagesIdPut(
    id,
    imageRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageRequest** | **ImageRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ImageReturn**

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

# **imagesPost**
> ImageReturn imagesPost()

Create an image

### Example

```typescript
import {
    StoreApi,
    Configuration,
    ImageRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let imageRequest: ImageRequest; // (optional)

const { status, data } = await apiInstance.imagesPost(
    imageRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageRequest** | **ImageRequest**|  | |


### Return type

**ImageReturn**

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

# **pointsGet**
> PointList pointsGet()

list points in database

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)

const { status, data } = await apiInstance.pointsGet(
    paginate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|


### Return type

**PointList**

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

# **pointsIdDelete**
> pointsIdDelete()

delete a point

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pointsIdDelete(
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

# **pointsIdGet**
> PointReturn pointsIdGet()

Information about a particular MRI coordinate

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pointsIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PointReturn**

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

# **pointsIdPut**
> PointReturn pointsIdPut()

Update a particular MRI coordinate.

### Example

```typescript
import {
    StoreApi,
    Configuration,
    PointRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let pointRequest: PointRequest; // (optional)

const { status, data } = await apiInstance.pointsIdPut(
    id,
    pointRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pointRequest** | **PointRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PointReturn**

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

# **pointsPost**
> PointReturn pointsPost()

add a point to an analysis

### Example

```typescript
import {
    StoreApi,
    Configuration,
    PointRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let pointRequest: PointRequest; // (optional)

const { status, data } = await apiInstance.pointsPost(
    pointRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pointRequest** | **PointRequest**|  | |


### Return type

**PointReturn**

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
let gzip: boolean; //return the content as gzipped content (optional) (default to undefined)

const { status, data } = await apiInstance.studysetsIdGet(
    id,
    nested,
    gzip
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|
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

# **tablesGet**
> TableList tablesGet()

List all tables across studies.

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
let name: string; //search the name field for a term (optional) (default to undefined)
let description: string; //search description field for a term (optional) (default to undefined)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)

const { status, data } = await apiInstance.tablesGet(
    search,
    sort,
    page,
    desc,
    pageSize,
    paginate,
    name,
    description,
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
| **name** | [**string**] | search the name field for a term | (optional) defaults to undefined|
| **description** | [**string**] | search description field for a term | (optional) defaults to undefined|
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|


### Return type

**TableList**

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

# **tablesIdDelete**
> tablesIdDelete()

delete a table

### Example

```typescript
import {
    StoreApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.tablesIdDelete(
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

# **tablesIdGet**
> TableReturn tablesIdGet()

Information about a specific table.

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

const { status, data } = await apiInstance.tablesIdGet(
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

**TableReturn**

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

# **tablesIdPut**
> TableReturn tablesIdPut()

update a table

### Example

```typescript
import {
    StoreApi,
    Configuration,
    TableRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let id: string; // (default to undefined)
let tableRequest: TableRequest; // (optional)

const { status, data } = await apiInstance.tablesIdPut(
    id,
    tableRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tableRequest** | **TableRequest**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**TableReturn**

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

# **tablesPost**
> TableReturn tablesPost()

create a table

### Example

```typescript
import {
    StoreApi,
    Configuration,
    TableRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StoreApi(configuration);

let tableRequest: TableRequest; // (optional)

const { status, data } = await apiInstance.tablesPost(
    tableRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tableRequest** | **TableRequest**|  | |


### Return type

**TableReturn**

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

