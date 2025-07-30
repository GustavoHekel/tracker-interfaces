# InsurersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**insurersControllerCreate**](#insurerscontrollercreate) | **POST** /insurers | Create insurer|
|[**insurersControllerFindAll**](#insurerscontrollerfindall) | **GET** /insurers | List all insurers|
|[**insurersControllerFindOne**](#insurerscontrollerfindone) | **GET** /insurers/{id} | Get an insurer by id|
|[**insurersControllerRemove**](#insurerscontrollerremove) | **DELETE** /insurers/{id} | Delete an insurer|
|[**insurersControllerUpdate**](#insurerscontrollerupdate) | **PATCH** /insurers/{id} | Update an insurer|

# **insurersControllerCreate**
> Insurer insurersControllerCreate(createInsurerDto)


### Example

```typescript
import {
    InsurersApi,
    Configuration,
    CreateInsurerDto
} from './api';

const configuration = new Configuration();
const apiInstance = new InsurersApi(configuration);

let createInsurerDto: CreateInsurerDto; //

const { status, data } = await apiInstance.insurersControllerCreate(
    createInsurerDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createInsurerDto** | **CreateInsurerDto**|  | |


### Return type

**Insurer**

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

# **insurersControllerFindAll**
> Array<Insurer> insurersControllerFindAll()


### Example

```typescript
import {
    InsurersApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InsurersApi(configuration);

const { status, data } = await apiInstance.insurersControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Insurer>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all insurers |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **insurersControllerFindOne**
> Insurer insurersControllerFindOne()


### Example

```typescript
import {
    InsurersApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InsurersApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.insurersControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Insurer**

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

# **insurersControllerRemove**
> insurersControllerRemove()


### Example

```typescript
import {
    InsurersApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InsurersApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.insurersControllerRemove(
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

# **insurersControllerUpdate**
> Insurer insurersControllerUpdate(updateInsurerDto)


### Example

```typescript
import {
    InsurersApi,
    Configuration,
    UpdateInsurerDto
} from './api';

const configuration = new Configuration();
const apiInstance = new InsurersApi(configuration);

let id: string; // (default to undefined)
let updateInsurerDto: UpdateInsurerDto; //

const { status, data } = await apiInstance.insurersControllerUpdate(
    id,
    updateInsurerDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateInsurerDto** | **UpdateInsurerDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Insurer**

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

