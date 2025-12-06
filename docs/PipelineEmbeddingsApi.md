# PipelineEmbeddingsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**pipelineEmbeddingsGet**](#pipelineembeddingsget) | **GET** /pipeline-embeddings/ | List pipeline embeddings|
|[**pipelineEmbeddingsIdGet**](#pipelineembeddingsidget) | **GET** /pipeline-embeddings/{id} | Get a pipeline embedding by id|

# **pipelineEmbeddingsGet**
> PipelineEmbeddingList pipelineEmbeddingsGet()


### Example

```typescript
import {
    PipelineEmbeddingsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineEmbeddingsApi(configuration);

let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)

const { status, data } = await apiInstance.pipelineEmbeddingsGet(
    paginate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|


### Return type

**PipelineEmbeddingList**

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

# **pipelineEmbeddingsIdGet**
> PipelineEmbedding pipelineEmbeddingsIdGet()


### Example

```typescript
import {
    PipelineEmbeddingsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelineEmbeddingsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pipelineEmbeddingsIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PipelineEmbedding**

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

