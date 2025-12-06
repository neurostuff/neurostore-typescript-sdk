# ImagesApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**imagesGet**](#imagesget) | **GET** /images/ | GET a list of images|
|[**imagesIdDelete**](#imagesiddelete) | **DELETE** /images/{id} | DELETE an image|
|[**imagesIdGet**](#imagesidget) | **GET** /images/{id} | GET an image|
|[**imagesIdPut**](#imagesidput) | **PUT** /images/{id} | PUT/update an image|
|[**imagesPost**](#imagespost) | **POST** /images/ | POST/create an image|

# **imagesGet**
> ImageList imagesGet()

Retrieve and list images.

### Example

```typescript
import {
    ImagesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

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
    ImagesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

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
    ImagesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

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
    ImagesApi,
    Configuration,
    ImageRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

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
    ImagesApi,
    Configuration,
    ImageRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

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

