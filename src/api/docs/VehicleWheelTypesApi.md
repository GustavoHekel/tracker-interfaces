# VehicleWheelTypesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vehicleWheelTypesControllerFindAll**](#vehiclewheeltypescontrollerfindall) | **GET** /vehicle-wheel-types | List all vehicle wheel types|
|[**vehicleWheelTypesControllerFindOne**](#vehiclewheeltypescontrollerfindone) | **GET** /vehicle-wheel-types/{id} | Get a vehicle wheel type by id|

# **vehicleWheelTypesControllerFindAll**
> Array<VehicleWheelType> vehicleWheelTypesControllerFindAll()


### Example

```typescript
import {
    VehicleWheelTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleWheelTypesApi(configuration);

const { status, data } = await apiInstance.vehicleWheelTypesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<VehicleWheelType>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all vehicle wheel types |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **vehicleWheelTypesControllerFindOne**
> VehicleWheelType vehicleWheelTypesControllerFindOne()


### Example

```typescript
import {
    VehicleWheelTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleWheelTypesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleWheelTypesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleWheelType**

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

