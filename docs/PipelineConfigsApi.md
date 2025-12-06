# PipelineConfigsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**pipelineConfigsGet**](#pipelineconfigsget) | **GET** /pipeline-configs/ | GET a list of pipeline configs|
|[**pipelineConfigsIdDelete**](#pipelineconfigsiddelete) | **DELETE** /pipeline-configs/{id} | DELETE a pipeline config by ID|
|[**pipelineConfigsIdGet**](#pipelineconfigsidget) | **GET** /pipeline-configs/{id} | GET a pipeline config by ID|
|[**pipelineConfigsIdPut**](#pipelineconfigsidput) | **PUT** /pipeline-configs/{id} | PUT/update a pipeline config by ID|
|[**pipelineConfigsPost**](#pipelineconfigspost) | **POST** /pipeline-configs/ | POST/create a pipeline config|

# **pipelineConfigsGet**
> PipelineConfigList pipelineConfigsGet()


### Example

```typescript
import {
    PipelineConfigsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineConfigsApi(configuration);

let pipeline: Array<string>; //Filter configs by pipeline name (optional) (default to undefined)
let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)
let hasEmbeddings: boolean; //Filter configs as whether they have embeddings saved. (optional) (default to undefined)
let embeddingDimensions: number; //Filter configs by number of dimensions in the embeddings. (optional) (default to undefined)

const { status, data } = await apiInstance.pipelineConfigsGet(
    pipeline,
    paginate,
    hasEmbeddings,
    embeddingDimensions
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipeline** | **Array&lt;string&gt;** | Filter configs by pipeline name | (optional) defaults to undefined|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|
| **hasEmbeddings** | [**boolean**] | Filter configs as whether they have embeddings saved. | (optional) defaults to undefined|
| **embeddingDimensions** | [**number**] | Filter configs by number of dimensions in the embeddings. | (optional) defaults to undefined|


### Return type

**PipelineConfigList**

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

# **pipelineConfigsIdDelete**
> pipelineConfigsIdDelete()


### Example

```typescript
import {
    PipelineConfigsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineConfigsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pipelineConfigsIdDelete(
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

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **pipelineConfigsIdGet**
> PipelineConfig pipelineConfigsIdGet()


### Example

```typescript
import {
    PipelineConfigsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineConfigsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pipelineConfigsIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PipelineConfig**

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

# **pipelineConfigsIdPut**
> pipelineConfigsIdPut()


### Example

```typescript
import {
    PipelineConfigsApi,
    Configuration,
    PipelineConfig
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineConfigsApi(configuration);

let id: string; // (default to undefined)
let pipelineConfig: PipelineConfig; // (optional)

const { status, data } = await apiInstance.pipelineConfigsIdPut(
    id,
    pipelineConfig
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipelineConfig** | **PipelineConfig**|  | |
| **id** | [**string**] |  | defaults to undefined|


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

# **pipelineConfigsPost**
> pipelineConfigsPost()


### Example

```typescript
import {
    PipelineConfigsApi,
    Configuration,
    PipelineConfig
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineConfigsApi(configuration);

let pipelineConfig: PipelineConfig; // (optional)

const { status, data } = await apiInstance.pipelineConfigsPost(
    pipelineConfig
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipelineConfig** | **PipelineConfig**|  | |


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
|**201** | Created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

