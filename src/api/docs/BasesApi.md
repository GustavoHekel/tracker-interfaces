# BasesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**basesControllerCreate**](#basescontrollercreate) | **POST** /bases | Create base|
|[**basesControllerFindAll**](#basescontrollerfindall) | **GET** /bases | List all bases|
|[**basesControllerFindOne**](#basescontrollerfindone) | **GET** /bases/{id} | Get a base by id|
|[**basesControllerRemove**](#basescontrollerremove) | **DELETE** /bases/{id} | Delete a base|
|[**basesControllerUpdate**](#basescontrollerupdate) | **PATCH** /bases/{id} | Update a base|

# **basesControllerCreate**
> Base basesControllerCreate(createBaseDto)


### Example

```typescript
import {
    BasesApi,
    Configuration,
    CreateBaseDto
} from './api';

const configuration = new Configuration();
const apiInstance = new BasesApi(configuration);

let createBaseDto: CreateBaseDto; //

const { status, data } = await apiInstance.basesControllerCreate(
    createBaseDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createBaseDto** | **CreateBaseDto**|  | |


### Return type

**Base**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | The record has been successfully created. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **basesControllerFindAll**
> Array<Base> basesControllerFindAll()


### Example

```typescript
import {
    BasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new BasesApi(configuration);

const { status, data } = await apiInstance.basesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Base>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all bases. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **basesControllerFindOne**
> Base basesControllerFindOne()


### Example

```typescript
import {
    BasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new BasesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.basesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Base**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The found record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **basesControllerRemove**
> basesControllerRemove()


### Example

```typescript
import {
    BasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new BasesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.basesControllerRemove(
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

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | The record has been successfully deleted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **basesControllerUpdate**
> Base basesControllerUpdate(body)


### Example

```typescript
import {
    BasesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new BasesApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.basesControllerUpdate(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Base**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The updated record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

