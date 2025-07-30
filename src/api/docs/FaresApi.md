# FaresApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**faresControllerCreate**](#farescontrollercreate) | **POST** /fares | |
|[**faresControllerFindAll**](#farescontrollerfindall) | **GET** /fares | |
|[**faresControllerFindOne**](#farescontrollerfindone) | **GET** /fares/{id} | |
|[**faresControllerRemove**](#farescontrollerremove) | **DELETE** /fares/{id} | |
|[**faresControllerUpdate**](#farescontrollerupdate) | **PATCH** /fares/{id} | |

# **faresControllerCreate**
> faresControllerCreate(body)


### Example

```typescript
import {
    FaresApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new FaresApi(configuration);

let body: object; //

const { status, data } = await apiInstance.faresControllerCreate(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |


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
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **faresControllerFindAll**
> faresControllerFindAll()


### Example

```typescript
import {
    FaresApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new FaresApi(configuration);

const { status, data } = await apiInstance.faresControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


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
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **faresControllerFindOne**
> faresControllerFindOne()


### Example

```typescript
import {
    FaresApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new FaresApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.faresControllerFindOne(
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
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **faresControllerRemove**
> faresControllerRemove()


### Example

```typescript
import {
    FaresApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new FaresApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.faresControllerRemove(
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
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **faresControllerUpdate**
> faresControllerUpdate(body)


### Example

```typescript
import {
    FaresApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new FaresApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.faresControllerUpdate(
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

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

