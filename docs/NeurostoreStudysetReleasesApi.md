# NeurostoreStudysetReleasesApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**neurostoreStudysetReleasesGet**](#neurostorestudysetreleasesget) | **GET** /neurostore-studyset-releases/ | GET NeuroStore studyset release list|
|[**neurostoreStudysetReleasesVersionDownloadGet**](#neurostorestudysetreleasesversiondownloadget) | **GET** /neurostore-studyset-releases/{version}/download | Download NeuroStore studyset release tarball|
|[**neurostoreStudysetReleasesVersionGet**](#neurostorestudysetreleasesversionget) | **GET** /neurostore-studyset-releases/{version} | GET NeuroStore studyset release manifest|

# **neurostoreStudysetReleasesGet**
> NeurostoreStudysetReleasesGet200Response neurostoreStudysetReleasesGet()


### Example

```typescript
import {
    NeurostoreStudysetReleasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new NeurostoreStudysetReleasesApi(configuration);

const { status, data } = await apiInstance.neurostoreStudysetReleasesGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**NeurostoreStudysetReleasesGet200Response**

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

# **neurostoreStudysetReleasesVersionDownloadGet**
> File neurostoreStudysetReleasesVersionDownloadGet()


### Example

```typescript
import {
    NeurostoreStudysetReleasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new NeurostoreStudysetReleasesApi(configuration);

let version: string; //nightly, latest, or a monthly release in YYYY-MM format. (default to undefined)

const { status, data } = await apiInstance.neurostoreStudysetReleasesVersionDownloadGet(
    version
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **version** | [**string**] | nightly, latest, or a monthly release in YYYY-MM format. | defaults to undefined|


### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/gzip, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **neurostoreStudysetReleasesVersionGet**
> object neurostoreStudysetReleasesVersionGet()


### Example

```typescript
import {
    NeurostoreStudysetReleasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new NeurostoreStudysetReleasesApi(configuration);

let version: string; //nightly, latest, or a monthly release in YYYY-MM format. (default to undefined)

const { status, data } = await apiInstance.neurostoreStudysetReleasesVersionGet(
    version
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **version** | [**string**] | nightly, latest, or a monthly release in YYYY-MM format. | defaults to undefined|


### Return type

**object**

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

