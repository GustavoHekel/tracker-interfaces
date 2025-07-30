# VehicleBrandsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vehicleBrandsControllerCreate**](#vehiclebrandscontrollercreate) | **POST** /vehicle-brands | Create vehicle brand|
|[**vehicleBrandsControllerFindAll**](#vehiclebrandscontrollerfindall) | **GET** /vehicle-brands | List all vehicle brands|
|[**vehicleBrandsControllerFindOne**](#vehiclebrandscontrollerfindone) | **GET** /vehicle-brands/{id} | Get a vehicle brand by id|
|[**vehicleBrandsControllerRemove**](#vehiclebrandscontrollerremove) | **DELETE** /vehicle-brands/{id} | Delete a vehicle brand|
|[**vehicleBrandsControllerUpdate**](#vehiclebrandscontrollerupdate) | **PATCH** /vehicle-brands/{id} | Update a vehicle brand|

# **vehicleBrandsControllerCreate**
> VehicleBrand vehicleBrandsControllerCreate(createVehicleBrandDto)


### Example

```typescript
import {
    VehicleBrandsApi,
    Configuration,
    CreateVehicleBrandDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandsApi(configuration);

let createVehicleBrandDto: CreateVehicleBrandDto; //

const { status, data } = await apiInstance.vehicleBrandsControllerCreate(
    createVehicleBrandDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createVehicleBrandDto** | **CreateVehicleBrandDto**|  | |


### Return type

**VehicleBrand**

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

# **vehicleBrandsControllerFindAll**
> Array<VehicleBrand> vehicleBrandsControllerFindAll()


### Example

```typescript
import {
    VehicleBrandsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandsApi(configuration);

const { status, data } = await apiInstance.vehicleBrandsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<VehicleBrand>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all vehicle brands |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **vehicleBrandsControllerFindOne**
> VehicleBrand vehicleBrandsControllerFindOne()


### Example

```typescript
import {
    VehicleBrandsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleBrandsControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleBrand**

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

# **vehicleBrandsControllerRemove**
> vehicleBrandsControllerRemove()


### Example

```typescript
import {
    VehicleBrandsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.vehicleBrandsControllerRemove(
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

# **vehicleBrandsControllerUpdate**
> VehicleBrand vehicleBrandsControllerUpdate(updateVehicleBrandDto)


### Example

```typescript
import {
    VehicleBrandsApi,
    Configuration,
    UpdateVehicleBrandDto
} from './api';

const configuration = new Configuration();
const apiInstance = new VehicleBrandsApi(configuration);

let id: string; // (default to undefined)
let updateVehicleBrandDto: UpdateVehicleBrandDto; //

const { status, data } = await apiInstance.vehicleBrandsControllerUpdate(
    id,
    updateVehicleBrandDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateVehicleBrandDto** | **UpdateVehicleBrandDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**VehicleBrand**

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

