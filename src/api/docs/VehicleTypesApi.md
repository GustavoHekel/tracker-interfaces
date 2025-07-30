# VehicleTypesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vehicleTypesControllerCreate**](#vehicletypescontrollercreate) | **POST** /vehicle-types | Create vehicle type|
|[**vehicleTypesControllerFindAll**](#vehicletypescontrollerfindall) | **GET** /vehicle-types | List all vehicle types|
|[**vehicleTypesControllerFindOne**](#vehicletypescontrollerfindone) | **GET** /vehicle-types/{id} | Get a vehicle type by id|
|[**vehicleTypesControllerRemove**](#vehicletypescontrollerremove) | **DELETE** /vehicle-types/{id} | Delete a vehicle type|
|[**vehicleTypesControllerUpdate**](#vehicletypescontrollerupdate) | **PATCH** /vehicle-types/{id} | Update a vehicle type|

# **vehicleTypesControllerCreate**
> VehicleType vehicleTypesControllerCreate(createVehicleTypeDto)


### Example

```typescript
import {
    VehicleTypesApi,
    Configuration,
    CreateVehicleTypeDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleTypesApi(configuration);

let createVehicleTypeDto: CreateVehicleTypeDto; //

const { status, data } = await apiInstance.vehicleTypesControllerCreate(
    createVehicleTypeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createVehicleTypeDto** | **CreateVehicleTypeDto**|  | |


### Return type

**VehicleType**

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

# **vehicleTypesControllerFindAll**
> Array<VehicleType> vehicleTypesControllerFindAll()


### Example

```typescript
import {
    VehicleTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleTypesApi(configuration);

const { status, data } = await apiInstance.vehicleTypesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<VehicleType>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all vehicle types |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **vehicleTypesControllerFindOne**
> VehicleType vehicleTypesControllerFindOne()


### Example

```typescript
import {
    VehicleTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleTypesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleTypesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleType**

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

# **vehicleTypesControllerRemove**
> vehicleTypesControllerRemove()


### Example

```typescript
import {
    VehicleTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleTypesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleTypesControllerRemove(
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

# **vehicleTypesControllerUpdate**
> VehicleType vehicleTypesControllerUpdate(updateVehicleTypeDto)


### Example

```typescript
import {
    VehicleTypesApi,
    Configuration,
    UpdateVehicleTypeDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleTypesApi(configuration);

let id: string; // (default to undefined)
let updateVehicleTypeDto: UpdateVehicleTypeDto; //

const { status, data } = await apiInstance.vehicleTypesControllerUpdate(
    id,
    updateVehicleTypeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateVehicleTypeDto** | **UpdateVehicleTypeDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleType**

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

