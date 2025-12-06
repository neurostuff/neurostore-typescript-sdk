# PipelineStudyResultsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**pipelineStudyResultsGet**](#pipelinestudyresultsget) | **GET** /pipeline-study-results/ | GET a list of pipeline run results|
|[**pipelineStudyResultsPipelineStudyResultIdDelete**](#pipelinestudyresultspipelinestudyresultiddelete) | **DELETE** /pipeline-study-results/{pipeline_study_result_id} | DELETE a pipeline run result by ID|
|[**pipelineStudyResultsPipelineStudyResultIdGet**](#pipelinestudyresultspipelinestudyresultidget) | **GET** /pipeline-study-results/{pipeline_study_result_id} | GET a pipeline run result by ID|
|[**pipelineStudyResultsPipelineStudyResultIdPut**](#pipelinestudyresultspipelinestudyresultidput) | **PUT** /pipeline-study-results/{pipeline_study_result_id} | PUT/update a pipeline run result by ID|
|[**pipelineStudyResultsPost**](#pipelinestudyresultspost) | **POST** /pipeline-study-results/ | POST/create a pipeline run result|

# **pipelineStudyResultsGet**
> PipelineStudyResultList pipelineStudyResultsGet()


### Example

```typescript
import {
    PipelineStudyResultsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineStudyResultsApi(configuration);

let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)
let featureFilter: Array<string>; //Filter results by feature content. Format: \"PipelineName[:version]:field_path=value\". Examples:   - \"TestPipeline:1.0.0:groups.diagnosis=ADHD\" (specific version)   - \"TestPipeline:groups.diagnosis=ADHD\" (latest version)  Field path supports array notation with [], regex search with ~, and comparisons with =, >, <, >=, <=.  (optional) (default to undefined)
let featureFlatten: boolean; // (optional) (default to undefined)
let pipelineConfig: Array<string>; //Filter results by pipeline config content. Format: \"PipelineName[:version]:config_path=value\". Examples:   - \"TestPipeline:1.0.0:preprocessing.smoothing=8\" (specific version)   - \"TestPipeline:model.type=linear\" (latest version)  Config path supports array notation with [], regex search with ~, and comparisons with =, >, <, >=, <=.  (optional) (default to undefined)
let featureDisplay: Array<string>; //Filter results by pipeline name and optionally version. Format: \"pipeline_name[:version]\". Examples:   - \"TestPipeline\" (all results from pipeline)   - \"TestPipeline:1.0.0\" (results from specific version) Multiple values can be provided to get results from multiple pipelines/versions.  (optional) (default to undefined)
let studyId: Array<string>; //Filter results by base study ID (optional) (default to undefined)
let version: string; //Filter results by pipeline config version (optional) (default to undefined)

const { status, data } = await apiInstance.pipelineStudyResultsGet(
    paginate,
    featureFilter,
    featureFlatten,
    pipelineConfig,
    featureDisplay,
    studyId,
    version
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|
| **featureFilter** | **Array&lt;string&gt;** | Filter results by feature content. Format: \&quot;PipelineName[:version]:field_path&#x3D;value\&quot;. Examples:   - \&quot;TestPipeline:1.0.0:groups.diagnosis&#x3D;ADHD\&quot; (specific version)   - \&quot;TestPipeline:groups.diagnosis&#x3D;ADHD\&quot; (latest version)  Field path supports array notation with [], regex search with ~, and comparisons with &#x3D;, &gt;, &lt;, &gt;&#x3D;, &lt;&#x3D;.  | (optional) defaults to undefined|
| **featureFlatten** | [**boolean**] |  | (optional) defaults to undefined|
| **pipelineConfig** | **Array&lt;string&gt;** | Filter results by pipeline config content. Format: \&quot;PipelineName[:version]:config_path&#x3D;value\&quot;. Examples:   - \&quot;TestPipeline:1.0.0:preprocessing.smoothing&#x3D;8\&quot; (specific version)   - \&quot;TestPipeline:model.type&#x3D;linear\&quot; (latest version)  Config path supports array notation with [], regex search with ~, and comparisons with &#x3D;, &gt;, &lt;, &gt;&#x3D;, &lt;&#x3D;.  | (optional) defaults to undefined|
| **featureDisplay** | **Array&lt;string&gt;** | Filter results by pipeline name and optionally version. Format: \&quot;pipeline_name[:version]\&quot;. Examples:   - \&quot;TestPipeline\&quot; (all results from pipeline)   - \&quot;TestPipeline:1.0.0\&quot; (results from specific version) Multiple values can be provided to get results from multiple pipelines/versions.  | (optional) defaults to undefined|
| **studyId** | **Array&lt;string&gt;** | Filter results by base study ID | (optional) defaults to undefined|
| **version** | [**string**] | Filter results by pipeline config version | (optional) defaults to undefined|


### Return type

**PipelineStudyResultList**

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

# **pipelineStudyResultsPipelineStudyResultIdDelete**
> pipelineStudyResultsPipelineStudyResultIdDelete()


### Example

```typescript
import {
    PipelineStudyResultsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineStudyResultsApi(configuration);

let pipelineStudyResultId: string; // (default to undefined)

const { status, data } = await apiInstance.pipelineStudyResultsPipelineStudyResultIdDelete(
    pipelineStudyResultId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipelineStudyResultId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **pipelineStudyResultsPipelineStudyResultIdGet**
> PipelineStudyResult pipelineStudyResultsPipelineStudyResultIdGet()


### Example

```typescript
import {
    PipelineStudyResultsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineStudyResultsApi(configuration);

let pipelineStudyResultId: string; // (default to undefined)

const { status, data } = await apiInstance.pipelineStudyResultsPipelineStudyResultIdGet(
    pipelineStudyResultId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipelineStudyResultId** | [**string**] |  | defaults to undefined|


### Return type

**PipelineStudyResult**

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

# **pipelineStudyResultsPipelineStudyResultIdPut**
> pipelineStudyResultsPipelineStudyResultIdPut()


### Example

```typescript
import {
    PipelineStudyResultsApi,
    Configuration,
    PipelineStudyResult
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineStudyResultsApi(configuration);

let pipelineStudyResultId: string; // (default to undefined)
let pipelineStudyResult: PipelineStudyResult; // (optional)

const { status, data } = await apiInstance.pipelineStudyResultsPipelineStudyResultIdPut(
    pipelineStudyResultId,
    pipelineStudyResult
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipelineStudyResult** | **PipelineStudyResult**|  | |
| **pipelineStudyResultId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **pipelineStudyResultsPost**
> PipelineStudyResultList pipelineStudyResultsPost()


### Example

```typescript
import {
    PipelineStudyResultsApi,
    Configuration,
    PipelineStudyResultPost
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineStudyResultsApi(configuration);

let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)
let featureFilter: Array<string>; //Filter results by feature content. Format: \"PipelineName[:version]:field_path=value\". Examples:   - \"TestPipeline:1.0.0:groups.diagnosis=ADHD\" (specific version)   - \"TestPipeline:groups.diagnosis=ADHD\" (latest version)  Field path supports array notation with [], regex search with ~, and comparisons with =, >, <, >=, <=.  (optional) (default to undefined)
let featureFlatten: boolean; // (optional) (default to undefined)
let pipelineConfig: Array<string>; //Filter results by pipeline config content. Format: \"PipelineName[:version]:config_path=value\". Examples:   - \"TestPipeline:1.0.0:preprocessing.smoothing=8\" (specific version)   - \"TestPipeline:model.type=linear\" (latest version)  Config path supports array notation with [], regex search with ~, and comparisons with =, >, <, >=, <=.  (optional) (default to undefined)
let featureDisplay: Array<string>; //Filter results by pipeline name and optionally version. Format: \"pipeline_name[:version]\". Examples:   - \"TestPipeline\" (all results from pipeline)   - \"TestPipeline:1.0.0\" (results from specific version) Multiple values can be provided to get results from multiple pipelines/versions.  (optional) (default to undefined)
let studyId: Array<string>; //Filter results by base study ID (optional) (default to undefined)
let version: string; //Filter results by pipeline config version (optional) (default to undefined)
let pipelineStudyResultPost: PipelineStudyResultPost; // (optional)

const { status, data } = await apiInstance.pipelineStudyResultsPost(
    paginate,
    featureFilter,
    featureFlatten,
    pipelineConfig,
    featureDisplay,
    studyId,
    version,
    pipelineStudyResultPost
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipelineStudyResultPost** | **PipelineStudyResultPost**|  | |
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|
| **featureFilter** | **Array&lt;string&gt;** | Filter results by feature content. Format: \&quot;PipelineName[:version]:field_path&#x3D;value\&quot;. Examples:   - \&quot;TestPipeline:1.0.0:groups.diagnosis&#x3D;ADHD\&quot; (specific version)   - \&quot;TestPipeline:groups.diagnosis&#x3D;ADHD\&quot; (latest version)  Field path supports array notation with [], regex search with ~, and comparisons with &#x3D;, &gt;, &lt;, &gt;&#x3D;, &lt;&#x3D;.  | (optional) defaults to undefined|
| **featureFlatten** | [**boolean**] |  | (optional) defaults to undefined|
| **pipelineConfig** | **Array&lt;string&gt;** | Filter results by pipeline config content. Format: \&quot;PipelineName[:version]:config_path&#x3D;value\&quot;. Examples:   - \&quot;TestPipeline:1.0.0:preprocessing.smoothing&#x3D;8\&quot; (specific version)   - \&quot;TestPipeline:model.type&#x3D;linear\&quot; (latest version)  Config path supports array notation with [], regex search with ~, and comparisons with &#x3D;, &gt;, &lt;, &gt;&#x3D;, &lt;&#x3D;.  | (optional) defaults to undefined|
| **featureDisplay** | **Array&lt;string&gt;** | Filter results by pipeline name and optionally version. Format: \&quot;pipeline_name[:version]\&quot;. Examples:   - \&quot;TestPipeline\&quot; (all results from pipeline)   - \&quot;TestPipeline:1.0.0\&quot; (results from specific version) Multiple values can be provided to get results from multiple pipelines/versions.  | (optional) defaults to undefined|
| **studyId** | **Array&lt;string&gt;** | Filter results by base study ID | (optional) defaults to undefined|
| **version** | [**string**] | Filter results by pipeline config version | (optional) defaults to undefined|


### Return type

**PipelineStudyResultList**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**200** | OK (search results) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

