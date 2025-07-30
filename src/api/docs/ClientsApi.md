# ClientsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**clientsControllerCreate**](#clientscontrollercreate) | **POST** /clients | Create client|
|[**clientsControllerFindAll**](#clientscontrollerfindall) | **GET** /clients | List all clients|
|[**clientsControllerFindOne**](#clientscontrollerfindone) | **GET** /clients/{id} | Get a client by id|
|[**clientsControllerRemove**](#clientscontrollerremove) | **DELETE** /clients/{id} | Delete a client|
|[**clientsControllerUpdate**](#clientscontrollerupdate) | **PATCH** /clients/{id} | Update a client|

# **clientsControllerCreate**
> Client clientsControllerCreate(createClientDto)


### Example

```typescript
import {
    ClientsApi,
    Configuration,
    CreateClientDto
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientsApi(configuration);

let createClientDto: CreateClientDto; //

const { status, data } = await apiInstance.clientsControllerCreate(
    createClientDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createClientDto** | **CreateClientDto**|  | |


### Return type

**Client**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | The record has been successfully created. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **clientsControllerFindAll**
> Array<Client> clientsControllerFindAll()


### Example

```typescript
import {
    ClientsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientsApi(configuration);

const { status, data } = await apiInstance.clientsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Client>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all clients |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **clientsControllerFindOne**
> Client clientsControllerFindOne()


### Example

```typescript
import {
    ClientsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.clientsControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Client**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The found record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **clientsControllerRemove**
> clientsControllerRemove()


### Example

```typescript
import {
    ClientsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.clientsControllerRemove(
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
|**200** | The deleted record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **clientsControllerUpdate**
> Client clientsControllerUpdate(body)


### Example

```typescript
import {
    ClientsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientsApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.clientsControllerUpdate(
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

**Client**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The updated record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

