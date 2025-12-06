# TablesApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**tablesGet**](#tablesget) | **GET** /tables/ | GET list of tables|
|[**tablesIdDelete**](#tablesiddelete) | **DELETE** /tables/{id} | DELETE a table|
|[**tablesIdGet**](#tablesidget) | **GET** /tables/{id} | GET a table|
|[**tablesIdPut**](#tablesidput) | **PUT** /tables/{id} | PUT/update a table|
|[**tablesPost**](#tablespost) | **POST** /tables/ | POST/create a table|

# **tablesGet**
> TableList tablesGet()

List all tables across studies.

### Example

```typescript
import {
    TablesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TablesApi(configuration);

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
    TablesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TablesApi(configuration);

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
    TablesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TablesApi(configuration);

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
    TablesApi,
    Configuration,
    TableRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new TablesApi(configuration);

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
    TablesApi,
    Configuration,
    TableRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new TablesApi(configuration);

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

