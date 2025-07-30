# LocationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**locationsControllerCreate**](#locationscontrollercreate) | **POST** /locations | Create location|
|[**locationsControllerFindAll**](#locationscontrollerfindall) | **GET** /locations | List all locations|
|[**locationsControllerFindOne**](#locationscontrollerfindone) | **GET** /locations/{id} | Get a location by id|
|[**locationsControllerRemove**](#locationscontrollerremove) | **DELETE** /locations/{id} | Delete a location|
|[**locationsControllerUpdate**](#locationscontrollerupdate) | **PATCH** /locations/{id} | Update a location|

# **locationsControllerCreate**
> locationsControllerCreate(createLocationDto)


### Example

```typescript
import {
    LocationsApi,
    Configuration,
    CreateLocationDto
} from './api';

const configuration = new Configuration();
const apiInstance = new LocationsApi(configuration);

let createLocationDto: CreateLocationDto; //

const { status, data } = await apiInstance.locationsControllerCreate(
    createLocationDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLocationDto** | **CreateLocationDto**|  | |


### Return type

void (empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**202** | Location creation request accepted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **locationsControllerFindAll**
> Array<Location> locationsControllerFindAll()


### Example

```typescript
import {
    LocationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LocationsApi(configuration);

const { status, data } = await apiInstance.locationsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Location>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all locations. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **locationsControllerFindOne**
> Location locationsControllerFindOne()


### Example

```typescript
import {
    LocationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LocationsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.locationsControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Location**

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

# **locationsControllerRemove**
> locationsControllerRemove()


### Example

```typescript
import {
    LocationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LocationsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.locationsControllerRemove(
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

# **locationsControllerUpdate**
> Location locationsControllerUpdate(body)


### Example

```typescript
import {
    LocationsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LocationsApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.locationsControllerUpdate(
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

**Location**

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

