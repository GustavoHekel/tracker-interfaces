# CranesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**cranesControllerAssign**](#cranescontrollerassign) | **POST** /cranes/assign | Assign a crane to a user|
|[**cranesControllerCreate**](#cranescontrollercreate) | **POST** /cranes | Create crane|
|[**cranesControllerDistanceToPoint**](#cranescontrollerdistancetopoint) | **GET** /cranes/distanceToPoint | Calculate distance to a point|
|[**cranesControllerDistanceToPointApi**](#cranescontrollerdistancetopointapi) | **GET** /cranes/distance-to-point-api | Calculate distance to a point using an external API|
|[**cranesControllerDistanceToPointByCrane**](#cranescontrollerdistancetopointbycrane) | **GET** /cranes/{id}/distance-to-point | Calculate distance to a point for a specific crane|
|[**cranesControllerFindAll**](#cranescontrollerfindall) | **GET** /cranes | List all cranes|
|[**cranesControllerFindOne**](#cranescontrollerfindone) | **GET** /cranes/{id} | Get a crane by id|
|[**cranesControllerGetAllCranesLocations**](#cranescontrollergetallcraneslocations) | **GET** /cranes/locations | Get all crane locations|
|[**cranesControllerGetCraneHistory**](#cranescontrollergetcranehistory) | **GET** /cranes/historyAssigned/{id} | Get the assignment history of a crane|
|[**cranesControllerGetCranesDriveFinished**](#cranescontrollergetcranesdrivefinished) | **GET** /cranes/cranesDriveFinished | Get cranes with finished drives|
|[**cranesControllerGetCranesStatus**](#cranescontrollergetcranesstatus) | **GET** /cranes/cranesStatus | Get the status of all cranes|
|[**cranesControllerRemove**](#cranescontrollerremove) | **DELETE** /cranes/{id} | Delete a crane|
|[**cranesControllerTickets**](#cranescontrollertickets) | **GET** /cranes/tickets | Get tickets for a crane|
|[**cranesControllerUnassign**](#cranescontrollerunassign) | **POST** /cranes/unassign | Unassign a crane from a user|
|[**cranesControllerUpdate**](#cranescontrollerupdate) | **PATCH** /cranes/{id} | Update a crane|

# **cranesControllerAssign**
> cranesControllerAssign(assignCraneDto)


### Example

```typescript
import {
    CranesApi,
    Configuration,
    AssignCraneDto
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let assignCraneDto: AssignCraneDto; //

const { status, data } = await apiInstance.cranesControllerAssign(
    assignCraneDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **assignCraneDto** | **AssignCraneDto**|  | |


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
|**201** | The crane has been successfully assigned. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerCreate**
> Crane cranesControllerCreate(createCraneDto)


### Example

```typescript
import {
    CranesApi,
    Configuration,
    CreateCraneDto
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let createCraneDto: CreateCraneDto; //

const { status, data } = await apiInstance.cranesControllerCreate(
    createCraneDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCraneDto** | **CreateCraneDto**|  | |


### Return type

**Crane**

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

# **cranesControllerDistanceToPoint**
> cranesControllerDistanceToPoint()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

const { status, data } = await apiInstance.cranesControllerDistanceToPoint();
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
|**200** | The distance to the point. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerDistanceToPointApi**
> cranesControllerDistanceToPointApi()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let craneId: number; // (default to undefined)
let lat: number; // (default to undefined)
let lng: number; // (default to undefined)
let currentTicketId: number; // (default to undefined)
let ticketTypeid: number; // (default to undefined)

const { status, data } = await apiInstance.cranesControllerDistanceToPointApi(
    craneId,
    lat,
    lng,
    currentTicketId,
    ticketTypeid
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **craneId** | [**number**] |  | defaults to undefined|
| **lat** | [**number**] |  | defaults to undefined|
| **lng** | [**number**] |  | defaults to undefined|
| **currentTicketId** | [**number**] |  | defaults to undefined|
| **ticketTypeid** | [**number**] |  | defaults to undefined|


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
|**200** | The distance to the point. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerDistanceToPointByCrane**
> cranesControllerDistanceToPointByCrane()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let id: string; // (default to undefined)
let lat: string; // (default to undefined)
let lng: string; // (default to undefined)

const { status, data } = await apiInstance.cranesControllerDistanceToPointByCrane(
    id,
    lat,
    lng
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **lat** | [**string**] |  | defaults to undefined|
| **lng** | [**string**] |  | defaults to undefined|


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
|**200** | The distance to the point. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerFindAll**
> Array<Crane> cranesControllerFindAll()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

const { status, data } = await apiInstance.cranesControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Crane>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A list of all cranes. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerFindOne**
> Crane cranesControllerFindOne()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.cranesControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Crane**

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

# **cranesControllerGetAllCranesLocations**
> cranesControllerGetAllCranesLocations()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

const { status, data } = await apiInstance.cranesControllerGetAllCranesLocations();
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
|**200** | A list of all crane locations. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerGetCraneHistory**
> cranesControllerGetCraneHistory()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.cranesControllerGetCraneHistory(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


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
|**200** | The assignment history of the crane. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerGetCranesDriveFinished**
> Array<CraneSummaryDto> cranesControllerGetCranesDriveFinished()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

const { status, data } = await apiInstance.cranesControllerGetCranesDriveFinished();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<CraneSummaryDto>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A list of cranes with finished drives. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerGetCranesStatus**
> Array<CranesStatusDto> cranesControllerGetCranesStatus()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

const { status, data } = await apiInstance.cranesControllerGetCranesStatus();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<CranesStatusDto>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The status of all cranes. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerRemove**
> cranesControllerRemove()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.cranesControllerRemove(
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

# **cranesControllerTickets**
> cranesControllerTickets()


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

const { status, data } = await apiInstance.cranesControllerTickets();
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
|**200** | A list of tickets for the crane. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerUnassign**
> cranesControllerUnassign(unassignCraneDto)


### Example

```typescript
import {
    CranesApi,
    Configuration,
    UnassignCraneDto
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let unassignCraneDto: UnassignCraneDto; //

const { status, data } = await apiInstance.cranesControllerUnassign(
    unassignCraneDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **unassignCraneDto** | **UnassignCraneDto**|  | |


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
|**201** | The crane has been successfully unassigned. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cranesControllerUpdate**
> Crane cranesControllerUpdate(body)


### Example

```typescript
import {
    CranesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CranesApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.cranesControllerUpdate(
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

**Crane**

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

