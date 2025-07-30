# DelaysApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**delaysControllerFindAllDelayValues**](#delayscontrollerfindalldelayvalues) | **GET** /delays/values | List all delay values|
|[**delaysControllerFindOneDelayValue**](#delayscontrollerfindonedelayvalue) | **GET** /delays/values/{id} | Get a delay value by id|

# **delaysControllerFindAllDelayValues**
> Array<DelayValue> delaysControllerFindAllDelayValues()


### Example

```typescript
import {
    DelaysApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DelaysApi(configuration);

const { status, data } = await apiInstance.delaysControllerFindAllDelayValues();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<DelayValue>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all delay values |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delaysControllerFindOneDelayValue**
> DelayValue delaysControllerFindOneDelayValue()


### Example

```typescript
import {
    DelaysApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DelaysApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.delaysControllerFindOneDelayValue(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**DelayValue**

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

