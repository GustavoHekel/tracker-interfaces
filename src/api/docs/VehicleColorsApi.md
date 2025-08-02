# VehicleColorsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vehicleColorsControllerCreate**](#vehiclecolorscontrollercreate) | **POST** /vehicle-colors | Create vehicle color|
|[**vehicleColorsControllerFindAll**](#vehiclecolorscontrollerfindall) | **GET** /vehicle-colors | List all vehicle colors|

# **vehicleColorsControllerCreate**
> VehicleColor vehicleColorsControllerCreate(createVehicleColorDto)


### Example

```typescript
import {
    VehicleColorsApi,
    Configuration,
    CreateVehicleColorDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleColorsApi(configuration);

let createVehicleColorDto: CreateVehicleColorDto; //

const { status, data } = await apiInstance.vehicleColorsControllerCreate(
    createVehicleColorDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createVehicleColorDto** | **CreateVehicleColorDto**|  | |


### Return type

**VehicleColor**

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

# **vehicleColorsControllerFindAll**
> Array<VehicleColor> vehicleColorsControllerFindAll()


### Example

```typescript
import {
    VehicleColorsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleColorsApi(configuration);

const { status, data } = await apiInstance.vehicleColorsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<VehicleColor>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all vehicle colors |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

