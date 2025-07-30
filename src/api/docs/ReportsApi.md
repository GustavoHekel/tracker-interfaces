# ReportsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**reportsControllerFindAll**](#reportscontrollerfindall) | **GET** /reports | List all reports|
|[**reportsControllerRequestTripsPerDay**](#reportscontrollerrequesttripsperday) | **POST** /reports/request-trips-per-day | Request trips per day report|
|[**reportsControllerRequestTripsStatusChanges**](#reportscontrollerrequesttripsstatuschanges) | **POST** /reports/request-trips-status-changes | Request trips status changes report|

# **reportsControllerFindAll**
> Array<Report> reportsControllerFindAll()


### Example

```typescript
import {
    ReportsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ReportsApi(configuration);

const { status, data } = await apiInstance.reportsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Report>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all reports. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reportsControllerRequestTripsPerDay**
> reportsControllerRequestTripsPerDay(tripsPerDayDto)


### Example

```typescript
import {
    ReportsApi,
    Configuration,
    TripsPerDayDto
} from './api';

const configuration = new Configuration();
const apiInstance = new ReportsApi(configuration);

let tripsPerDayDto: TripsPerDayDto; //

const { status, data } = await apiInstance.reportsControllerRequestTripsPerDay(
    tripsPerDayDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tripsPerDayDto** | **TripsPerDayDto**|  | |


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
|**201** | Trips per day report request accepted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reportsControllerRequestTripsStatusChanges**
> reportsControllerRequestTripsStatusChanges(tripsStatusChangesDto)


### Example

```typescript
import {
    ReportsApi,
    Configuration,
    TripsStatusChangesDto
} from './api';

const configuration = new Configuration();
const apiInstance = new ReportsApi(configuration);

let tripsStatusChangesDto: TripsStatusChangesDto; //

const { status, data } = await apiInstance.reportsControllerRequestTripsStatusChanges(
    tripsStatusChangesDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tripsStatusChangesDto** | **TripsStatusChangesDto**|  | |


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
|**201** | Trips status changes report request accepted. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

