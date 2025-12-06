# PipelinesApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**pipelinesGet**](#pipelinesget) | **GET** /pipelines/ | GET a list of pipelines|
|[**pipelinesIdDelete**](#pipelinesiddelete) | **DELETE** /pipelines/{id} | DELETE a pipeline by ID|
|[**pipelinesIdGet**](#pipelinesidget) | **GET** /pipelines/{id} | GET a pipeline by ID|
|[**pipelinesIdPut**](#pipelinesidput) | **PUT** /pipelines/{id} | PUT/update a pipeline by ID|
|[**pipelinesPost**](#pipelinespost) | **POST** /pipelines/ | POST/create a pipeline|

# **pipelinesGet**
> PipelineList pipelinesGet()


### Example

```typescript
import {
    PipelinesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelinesApi(configuration);

let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)

const { status, data } = await apiInstance.pipelinesGet(
    paginate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paginate** | [**boolean**] | whether to paginate results (true) or return all results at once (false) | (optional) defaults to true|


### Return type

**PipelineList**

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

# **pipelinesIdDelete**
> pipelinesIdDelete()


### Example

```typescript
import {
    PipelinesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelinesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pipelinesIdDelete(
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

# **pipelinesIdGet**
> Pipeline pipelinesIdGet()


### Example

```typescript
import {
    PipelinesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelinesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.pipelinesIdGet(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Pipeline**

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

# **pipelinesIdPut**
> pipelinesIdPut()


### Example

```typescript
import {
    PipelinesApi,
    Configuration,
    Pipeline
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelinesApi(configuration);

let id: string; // (default to undefined)
let pipeline: Pipeline; // (optional)

const { status, data } = await apiInstance.pipelinesIdPut(
    id,
    pipeline
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipeline** | **Pipeline**|  | |
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

# **pipelinesPost**
> pipelinesPost()


### Example

```typescript
import {
    PipelinesApi,
    Configuration,
    Pipeline
} from './api';

const configuration = new Configuration();
const apiInstance = new PipelinesApi(configuration);

let pipeline: Pipeline; // (optional)

const { status, data } = await apiInstance.pipelinesPost(
    pipeline
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pipeline** | **Pipeline**|  | |


### Return type

void (empty response body)

### Authorization

[JSON-Web-Token](../README.md#JSON-Web-Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**401** | Unauthorized - Authentication required |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

