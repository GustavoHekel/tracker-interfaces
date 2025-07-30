# GearBoxTypesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**gearBoxTypesControllerFindAll**](#gearboxtypescontrollerfindall) | **GET** /gear-box-types | List all gear box types|
|[**gearBoxTypesControllerFindOne**](#gearboxtypescontrollerfindone) | **GET** /gear-box-types/{id} | Get a gear box type by id|

# **gearBoxTypesControllerFindAll**
> Array<GearBoxType> gearBoxTypesControllerFindAll()


### Example

```typescript
import {
    GearBoxTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GearBoxTypesApi(configuration);

const { status, data } = await apiInstance.gearBoxTypesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<GearBoxType>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all gear box types |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **gearBoxTypesControllerFindOne**
> GearBoxType gearBoxTypesControllerFindOne()


### Example

```typescript
import {
    GearBoxTypesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GearBoxTypesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.gearBoxTypesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**GearBoxType**

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

