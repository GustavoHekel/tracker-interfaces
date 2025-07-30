# VehicleBrandModelsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vehicleBrandModelsControllerCreate**](#vehiclebrandmodelscontrollercreate) | **POST** /vehicle-brand-models | Create vehicle brand model|
|[**vehicleBrandModelsControllerFindAll**](#vehiclebrandmodelscontrollerfindall) | **GET** /vehicle-brand-models | List all vehicle brand models|
|[**vehicleBrandModelsControllerFindOne**](#vehiclebrandmodelscontrollerfindone) | **GET** /vehicle-brand-models/{id} | Get a vehicle brand model by id|
|[**vehicleBrandModelsControllerRemove**](#vehiclebrandmodelscontrollerremove) | **DELETE** /vehicle-brand-models/{id} | Delete a vehicle brand model|
|[**vehicleBrandModelsControllerUpdate**](#vehiclebrandmodelscontrollerupdate) | **PATCH** /vehicle-brand-models/{id} | Update a vehicle brand model|

# **vehicleBrandModelsControllerCreate**
> VehicleBrandModel vehicleBrandModelsControllerCreate(createVehicleBrandModelDto)


### Example

```typescript
import {
    VehicleBrandModelsApi,
    Configuration,
    CreateVehicleBrandModelDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandModelsApi(configuration);

let createVehicleBrandModelDto: CreateVehicleBrandModelDto; //

const { status, data } = await apiInstance.vehicleBrandModelsControllerCreate(
    createVehicleBrandModelDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createVehicleBrandModelDto** | **CreateVehicleBrandModelDto**|  | |


### Return type

**VehicleBrandModel**

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

# **vehicleBrandModelsControllerFindAll**
> Array<VehicleBrandModel> vehicleBrandModelsControllerFindAll()


### Example

```typescript
import {
    VehicleBrandModelsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandModelsApi(configuration);

const { status, data } = await apiInstance.vehicleBrandModelsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<VehicleBrandModel>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all vehicle brand models |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **vehicleBrandModelsControllerFindOne**
> VehicleBrandModel vehicleBrandModelsControllerFindOne()


### Example

```typescript
import {
    VehicleBrandModelsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandModelsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleBrandModelsControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleBrandModel**

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

# **vehicleBrandModelsControllerRemove**
> vehicleBrandModelsControllerRemove()


### Example

```typescript
import {
    VehicleBrandModelsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandModelsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleBrandModelsControllerRemove(
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

# **vehicleBrandModelsControllerUpdate**
> VehicleBrandModel vehicleBrandModelsControllerUpdate(updateVehicleBrandModelDto)


### Example

```typescript
import {
    VehicleBrandModelsApi,
    Configuration,
    UpdateVehicleBrandModelDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandModelsApi(configuration);

let id: string; // (default to undefined)
let updateVehicleBrandModelDto: UpdateVehicleBrandModelDto; //

const { status, data } = await apiInstance.vehicleBrandModelsControllerUpdate(
    id,
    updateVehicleBrandModelDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateVehicleBrandModelDto** | **UpdateVehicleBrandModelDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleBrandModel**

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

