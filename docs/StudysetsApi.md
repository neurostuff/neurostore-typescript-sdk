# StudysetsApi

All URIs are relative to *https://neurostore.org/api*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**studysetsGet**](#studysetsget) | **GET** /studysets/ | GET a list of studysets|

# **studysetsGet**
> StudysetList studysetsGet()

Get a list of studysets.

### Example

```typescript
import {
    StudysetsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new StudysetsApi(configuration);

let search: string; //search for entries that contain the substring (optional) (default to undefined)
let sort: string; //Parameter to sort results on (optional) (default to 'created_at')
let page: number; //page of results (optional) (default to undefined)
let desc: boolean; //sort results by descending order (as opposed to ascending order) (optional) (default to undefined)
let pageSize: number; //number of results to show on a page (optional) (default to undefined)
let paginate: boolean; //whether to paginate results (true) or return all results at once (false) (optional) (default to true)
let nested: boolean; //whether to show the URI to a resource (false) or to embed the object in the response (true) (optional) (default to undefined)
let name: string; //search the name field for a term (optional) (default to undefined)
let description: string; //search description field for a term (optional) (default to undefined)
let sourceId: string; //id of the resource you are either filtering/copying on (optional) (default to undefined)
let unique: any; //whether to list clones with originals (optional) (default to undefined)
let source: 'neurostore' | 'neurovault' | 'pubmed' | 'neurosynth' | 'neuroquery' | 'pubget'; //the source of the resource you would like to filter/copy from (optional) (default to 'neurostore')
let authors: string; //search authors (optional) (default to undefined)
let userId: string; //user id you want to filter by (optional) (default to undefined)

const { status, data } = await apiInstance.studysetsGet(
    search,
    sort,
    page,
    desc,
    pageSize,
    paginate,
    nested,
    name,
    description,
    sourceId,
    unique,
    source,
    authors,
    userId
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
| **nested** | [**boolean**] | whether to show the URI to a resource (false) or to embed the object in the response (true) | (optional) defaults to undefined|
| **name** | [**string**] | search the name field for a term | (optional) defaults to undefined|
| **description** | [**string**] | search description field for a term | (optional) defaults to undefined|
| **sourceId** | [**string**] | id of the resource you are either filtering/copying on | (optional) defaults to undefined|
| **unique** | **any** | whether to list clones with originals | (optional) defaults to undefined|
| **source** | [**&#39;neurostore&#39; | &#39;neurovault&#39; | &#39;pubmed&#39; | &#39;neurosynth&#39; | &#39;neuroquery&#39; | &#39;pubget&#39;**]**Array<&#39;neurostore&#39; &#124; &#39;neurovault&#39; &#124; &#39;pubmed&#39; &#124; &#39;neurosynth&#39; &#124; &#39;neuroquery&#39; &#124; &#39;pubget&#39;>** | the source of the resource you would like to filter/copy from | (optional) defaults to 'neurostore'|
| **authors** | [**string**] | search authors | (optional) defaults to undefined|
| **userId** | [**string**] | user id you want to filter by | (optional) defaults to undefined|


### Return type

**StudysetList**

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

