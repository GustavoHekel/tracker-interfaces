# SettingsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**settingsControllerCreate**](#settingscontrollercreate) | **POST** /settings | Create setting|
|[**settingsControllerFindAll**](#settingscontrollerfindall) | **GET** /settings | List all settings|
|[**settingsControllerFindOne**](#settingscontrollerfindone) | **GET** /settings/{id} | Get a setting by id|
|[**settingsControllerRemove**](#settingscontrollerremove) | **DELETE** /settings/{id} | Delete a setting|
|[**settingsControllerUpdate**](#settingscontrollerupdate) | **PATCH** /settings/{id} | Update a setting|

# **settingsControllerCreate**
> Setting settingsControllerCreate(createSettingDto)


### Example

```typescript
import {
    SettingsApi,
    Configuration,
    CreateSettingDto
} from './api';

const configuration = new Configuration();
const apiInstance = new SettingsApi(configuration);

let createSettingDto: CreateSettingDto; //

const { status, data } = await apiInstance.settingsControllerCreate(
    createSettingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createSettingDto** | **CreateSettingDto**|  | |


### Return type

**Setting**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | The record has been successfully created. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **settingsControllerFindAll**
> Array<Setting> settingsControllerFindAll()


### Example

```typescript
import {
    SettingsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettingsApi(configuration);

const { status, data } = await apiInstance.settingsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Setting>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all settings. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **settingsControllerFindOne**
> Setting settingsControllerFindOne()


### Example

```typescript
import {
    SettingsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettingsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.settingsControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Setting**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The found record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **settingsControllerRemove**
> settingsControllerRemove()


### Example

```typescript
import {
    SettingsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettingsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.settingsControllerRemove(
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

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | The record has been successfully deleted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **settingsControllerUpdate**
> Setting settingsControllerUpdate(body)


### Example

```typescript
import {
    SettingsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SettingsApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.settingsControllerUpdate(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Setting**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The updated record |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

