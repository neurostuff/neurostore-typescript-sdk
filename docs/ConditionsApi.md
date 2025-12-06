# ConditionsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**conditionsGet**](#conditionsget) | **GET** /conditions/ | GET Conditions|
|[**conditionsIdDelete**](#conditionsiddelete) | **DELETE** /conditions/{id} | DELETE a condition|
|[**conditionsIdGet**](#conditionsidget) | **GET** /conditions/{id} | GET a condition|
|[**conditionsIdPut**](#conditionsidput) | **PUT** /conditions/{id} | PUT/update a condition|
|[**conditionsPost**](#conditionspost) | **POST** /conditions/ | POST/Create a condition|

# **conditionsGet**
> ConditionList conditionsGet()

Get all conditions

### Example

```typescript
import {
    ConditionsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ConditionsApi(configuration);

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
    ConditionsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ConditionsApi(configuration);

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
    ConditionsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ConditionsApi(configuration);

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
    ConditionsApi,
    Configuration,
    ConditionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new ConditionsApi(configuration);

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
    ConditionsApi,
    Configuration,
    ConditionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new ConditionsApi(configuration);

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

