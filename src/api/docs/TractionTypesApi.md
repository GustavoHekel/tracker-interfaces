# TractionTypesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**tractionTypesControllerFindAll**](#tractiontypescontrollerfindall) | **GET** /traction-types | List all traction types|
|[**tractionTypesControllerFindOne**](#tractiontypescontrollerfindone) | **GET** /traction-types/{id} | Get a traction type by id|

# **tractionTypesControllerFindAll**
> Array<TractionType> tractionTypesControllerFindAll()


### Example

```typescript
import {
    TractionTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TractionTypesApi(configuration);

const { status, data } = await apiInstance.tractionTypesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<TractionType>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all traction types |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **tractionTypesControllerFindOne**
> TractionType tractionTypesControllerFindOne()


### Example

```typescript
import {
    TractionTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TractionTypesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.tractionTypesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**TractionType**

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

