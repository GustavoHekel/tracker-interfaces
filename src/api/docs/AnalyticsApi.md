# AnalyticsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**analyticsControllerGetEstimatedTrips**](#analyticscontrollergetestimatedtrips) | **GET** /analytics/estimated-trips | Get estimated trips|
|[**analyticsControllerGetTotalActiveCranesByStatus**](#analyticscontrollergettotalactivecranesbystatus) | **GET** /analytics/total-active-cranes-by-status | Get total active cranes by status|
|[**analyticsControllerGetTotalDistancePerDay**](#analyticscontrollergettotaldistanceperday) | **GET** /analytics/total-distance-per-day | Get total distance per day|
|[**analyticsControllerGetTotalTripsForCurrentDay**](#analyticscontrollergettotaltripsforcurrentday) | **GET** /analytics/total-trips-for-current-day | Get total trips for current day|
|[**analyticsControllerGetTotalTripsForCurrentMonth**](#analyticscontrollergettotaltripsforcurrentmonth) | **GET** /analytics/total-trips-for-current-month | Get total trips for current month|
|[**analyticsControllerGetTotalTripsPerInsuranceCompanyPerMonth**](#analyticscontrollergettotaltripsperinsurancecompanypermonth) | **GET** /analytics/total-trips-per-insurance-company-per-month | Get total trips per insurance company per month|
|[**analyticsControllerGetTotalTripsPerLocation**](#analyticscontrollergettotaltripsperlocation) | **GET** /analytics/total-trips-per-location | Get total trips per location|
|[**analyticsControllerGetTotalTripsPerType**](#analyticscontrollergettotaltripspertype) | **GET** /analytics/total-trips-per-type | Get total trips per type|
|[**analyticsControllerGetTotalTripsPerVehicleType**](#analyticscontrollergettotaltripspervehicletype) | **GET** /analytics/total-trips-per-vehicle-type | Get total trips per vehicle type|

# **analyticsControllerGetEstimatedTrips**
> analyticsControllerGetEstimatedTrips()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetEstimatedTrips();
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
|**200** | Estimated trips. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalActiveCranesByStatus**
> analyticsControllerGetTotalActiveCranesByStatus()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalActiveCranesByStatus();
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
|**200** | Total active cranes by status. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalDistancePerDay**
> analyticsControllerGetTotalDistancePerDay()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalDistancePerDay();
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
|**200** | Total distance per day. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalTripsForCurrentDay**
> analyticsControllerGetTotalTripsForCurrentDay()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalTripsForCurrentDay();
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
|**200** | Total trips for the current day. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalTripsForCurrentMonth**
> analyticsControllerGetTotalTripsForCurrentMonth()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalTripsForCurrentMonth();
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
|**200** | Total trips for the current month. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalTripsPerInsuranceCompanyPerMonth**
> analyticsControllerGetTotalTripsPerInsuranceCompanyPerMonth()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalTripsPerInsuranceCompanyPerMonth();
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
|**200** | Total trips per insurance company per month. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalTripsPerLocation**
> analyticsControllerGetTotalTripsPerLocation()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalTripsPerLocation();
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
|**200** | Total trips per location. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalTripsPerType**
> analyticsControllerGetTotalTripsPerType()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalTripsPerType();
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
|**200** | Total trips per type. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analyticsControllerGetTotalTripsPerVehicleType**
> analyticsControllerGetTotalTripsPerVehicleType()


### Example

```typescript
import {
    AnalyticsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AnalyticsApi(configuration);

const { status, data } = await apiInstance.analyticsControllerGetTotalTripsPerVehicleType();
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
|**200** | Total trips per vehicle type. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

