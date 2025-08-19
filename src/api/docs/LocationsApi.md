# LocationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**locationsControllerCreate**](#locationscontrollercreate) | **POST** /locations | Create location|
|[**locationsControllerFindAll**](#locationscontrollerfindall) | **GET** /locations | List all locations|
|[**locationsControllerFindOne**](#locationscontrollerfindone) | **GET** /locations/{id} | Get a location by id|

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
|**201** | Location creation request accepted. |  -  |

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

