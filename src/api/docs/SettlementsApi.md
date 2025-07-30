# SettlementsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**settlementsControllerCalculateForDrivers**](#settlementscontrollercalculatefordrivers) | **GET** /settlements/provider | Calculate settlements for providers (TODO: Remove)|
|[**settlementsControllerFindAll**](#settlementscontrollerfindall) | **GET** /settlements | List all settlements|
|[**settlementsControllerRequestEmail**](#settlementscontrollerrequestemail) | **POST** /settlements/request-email | Request settlement email|

# **settlementsControllerCalculateForDrivers**
> settlementsControllerCalculateForDrivers()


### Example

```typescript
import {
    SettlementsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettlementsApi(configuration);

const { status, data } = await apiInstance.settlementsControllerCalculateForDrivers();
```

### Parameters
This endpoint does not have any parameters.


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
|**200** | Settlements calculated. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **settlementsControllerFindAll**
> Array<Settlement> settlementsControllerFindAll()


### Example

```typescript
import {
    SettlementsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettlementsApi(configuration);

const { status, data } = await apiInstance.settlementsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Settlement>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all settlements. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **settlementsControllerRequestEmail**
> settlementsControllerRequestEmail(body)


### Example

```typescript
import {
    SettlementsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettlementsApi(configuration);

let body: object; //

const { status, data } = await apiInstance.settlementsControllerRequestEmail(
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

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Settlement email request accepted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

