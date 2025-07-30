# RolesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**rolesControllerCreate**](#rolescontrollercreate) | **POST** /roles | Create role|
|[**rolesControllerFindAll**](#rolescontrollerfindall) | **GET** /roles | List all roles|
|[**rolesControllerFindOne**](#rolescontrollerfindone) | **GET** /roles/{id} | Get a role by id|
|[**rolesControllerRemove**](#rolescontrollerremove) | **DELETE** /roles/{id} | Delete a role|
|[**rolesControllerUpdate**](#rolescontrollerupdate) | **PATCH** /roles/{id} | Update a role|

# **rolesControllerCreate**
> Role rolesControllerCreate(createRoleDto)


### Example

```typescript
import {
    RolesApi,
    Configuration,
    CreateRoleDto
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

let createRoleDto: CreateRoleDto; //

const { status, data } = await apiInstance.rolesControllerCreate(
    createRoleDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createRoleDto** | **CreateRoleDto**|  | |


### Return type

**Role**

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

# **rolesControllerFindAll**
> Array<Role> rolesControllerFindAll()


### Example

```typescript
import {
    RolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

const { status, data } = await apiInstance.rolesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Role>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all roles. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **rolesControllerFindOne**
> Role rolesControllerFindOne()


### Example

```typescript
import {
    RolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.rolesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Role**

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

# **rolesControllerRemove**
> rolesControllerRemove()


### Example

```typescript
import {
    RolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.rolesControllerRemove(
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

# **rolesControllerUpdate**
> Role rolesControllerUpdate(body)


### Example

```typescript
import {
    RolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.rolesControllerUpdate(
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

**Role**

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

