# StudiesApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**baseStudiesGet**](#basestudiesget) | **GET** /base-studies/ | |
|[**baseStudiesIdGet**](#basestudiesidget) | **GET** /base-studies/{id} | Your GET endpoint|
|[**baseStudiesIdPut**](#basestudiesidput) | **PUT** /base-studies/{id} | |
|[**baseStudiesPost**](#basestudiespost) | **POST** /base-studies/ | |

# **baseStudiesGet**
> BaseStudyList baseStudiesGet()


### Example

```typescript
import {
    StudiesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StudiesApi(configuration);

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
let mapType: 'z' | 't' | 'beta_variance' | 'any'; //filter by stored map-type flags (optional) (default to undefined)
let isOa: boolean; // (optional) (default to undefined)
let publication: string; //search for papers from a particular journal (optional) (default to undefined)
let pmid: string; //search for particular pmid (optional) (default to undefined)
let doi: string; //search for study with specific doi (optional) (default to undefined)
let neurovaultId: string; //search for study with specific neurovault id (optional) (default to undefined)
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
    mapType,
    isOa,
    publication,
    pmid,
    doi,
    neurovaultId,
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
| **mapType** | [**&#39;z&#39; | &#39;t&#39; | &#39;beta_variance&#39; | &#39;any&#39;**]**Array<&#39;z&#39; &#124; &#39;t&#39; &#124; &#39;beta_variance&#39; &#124; &#39;any&#39;>** | filter by stored map-type flags | (optional) defaults to undefined|
| **isOa** | [**boolean**] |  | (optional) defaults to undefined|
| **publication** | [**string**] | search for papers from a particular journal | (optional) defaults to undefined|
| **pmid** | [**string**] | search for particular pmid | (optional) defaults to undefined|
| **doi** | [**string**] | search for study with specific doi | (optional) defaults to undefined|
| **neurovaultId** | [**string**] | search for study with specific neurovault id | (optional) defaults to undefined|
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
    StudiesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StudiesApi(configuration);

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
    StudiesApi,
    Configuration,
    BaseStudy
} from './api';

const configuration = new Configuration();
const apiInstance = new StudiesApi(configuration);

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
    StudiesApi,
    Configuration,
    BaseStudiesPostRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new StudiesApi(configuration);

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

