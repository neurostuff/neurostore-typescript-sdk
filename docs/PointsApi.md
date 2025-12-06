# PointsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**pointsGet**](#pointsget) | **GET** /points/ | Get Points|
|[**pointsIdDelete**](#pointsiddelete) | **DELETE** /points/{id} | DELETE a point|
|[**pointsIdGet**](#pointsidget) | **GET** /points/{id} | GET a point|
|[**pointsIdPut**](#pointsidput) | **PUT** /points/{id} | PUT/update a point|
|[**pointsPost**](#pointspost) | **POST** /points/ | POST Points|

# **pointsGet**
> PointList pointsGet()

list points in database

### Example

```typescript
import {
    PointsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PointsApi(configuration);

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
    PointsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PointsApi(configuration);

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
    PointsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PointsApi(configuration);

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
    PointsApi,
    Configuration,
    PointRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new PointsApi(configuration);

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
    PointsApi,
    Configuration,
    PointRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new PointsApi(configuration);

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

