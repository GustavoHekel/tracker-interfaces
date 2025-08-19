# TicketsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**ticketsControllerAssign**](#ticketscontrollerassign) | **POST** /tickets/{ticketId}/assign/{craneId} | Assign a ticket to a crane|
|[**ticketsControllerCreate**](#ticketscontrollercreate) | **POST** /tickets | Create ticket|
|[**ticketsControllerCreateEventFromSir**](#ticketscontrollercreateeventfromsir) | **POST** /tickets/events/sir | Create event from SIR|
|[**ticketsControllerCreateTicketComment**](#ticketscontrollercreateticketcomment) | **POST** /tickets/comments | Create a ticket comment|
|[**ticketsControllerFindAll**](#ticketscontrollerfindall) | **GET** /tickets | List all tickets|
|[**ticketsControllerFindAllBeta**](#ticketscontrollerfindallbeta) | **GET** /tickets/beta | List all tickets (beta)|
|[**ticketsControllerFindOne**](#ticketscontrollerfindone) | **GET** /tickets/{id} | Get a ticket by id|
|[**ticketsControllerFindTickets**](#ticketscontrollerfindtickets) | **GET** /tickets/board | Find tickets for board|
|[**ticketsControllerFindTicketsByDriverId**](#ticketscontrollerfindticketsbydriverid) | **GET** /tickets/by-driver | List all tickets that belong to a driver|
|[**ticketsControllerGetArrivalTimeCrane**](#ticketscontrollergetarrivaltimecrane) | **GET** /tickets/arrival-time/{ticketId}/{craneId} | Get arrival time for a crane to a ticket|
|[**ticketsControllerGetNearbyCranes**](#ticketscontrollergetnearbycranes) | **GET** /tickets/{id}/nearby-cranes | Get nearby cranes for a ticket|
|[**ticketsControllerRemove**](#ticketscontrollerremove) | **DELETE** /tickets/{id} | Delete a ticket|
|[**ticketsControllerUpdate**](#ticketscontrollerupdate) | **PATCH** /tickets/{id} | Update a ticket|
|[**ticketsControllerUpdateTicketStep**](#ticketscontrollerupdateticketstep) | **PATCH** /tickets/step/{id} | Update a ticket step|

# **ticketsControllerAssign**
> ticketsControllerAssign()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let ticketId: string; // (default to undefined)
let craneId: string; // (default to undefined)

const { status, data } = await apiInstance.ticketsControllerAssign(
    ticketId,
    craneId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ticketId** | [**string**] |  | defaults to undefined|
| **craneId** | [**string**] |  | defaults to undefined|


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
|**201** | The ticket has been successfully assigned. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerCreate**
> Ticket ticketsControllerCreate(createTicketDto)


### Example

```typescript
import {
    TicketsApi,
    Configuration,
    CreateTicketDto
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let createTicketDto: CreateTicketDto; //

const { status, data } = await apiInstance.ticketsControllerCreate(
    createTicketDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTicketDto** | **CreateTicketDto**|  | |


### Return type

**Ticket**

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

# **ticketsControllerCreateEventFromSir**
> ticketsControllerCreateEventFromSir(sirEventDto)


### Example

```typescript
import {
    TicketsApi,
    Configuration,
    SirEventDto
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let sirEventDto: SirEventDto; //

const { status, data } = await apiInstance.ticketsControllerCreateEventFromSir(
    sirEventDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sirEventDto** | **SirEventDto**|  | |


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
|**201** | The event has been successfully created. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerCreateTicketComment**
> ticketsControllerCreateTicketComment(createTicketCommentDto)


### Example

```typescript
import {
    TicketsApi,
    Configuration,
    CreateTicketCommentDto
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let createTicketCommentDto: CreateTicketCommentDto; //

const { status, data } = await apiInstance.ticketsControllerCreateTicketComment(
    createTicketCommentDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTicketCommentDto** | **CreateTicketCommentDto**|  | |


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
|**201** | The comment has been successfully created. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerFindAll**
> Array<Ticket> ticketsControllerFindAll()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

const { status, data } = await apiInstance.ticketsControllerFindAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Ticket>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all tickets. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerFindAllBeta**
> Array<Ticket> ticketsControllerFindAllBeta()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

const { status, data } = await apiInstance.ticketsControllerFindAllBeta();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Ticket>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all tickets. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerFindOne**
> Ticket ticketsControllerFindOne()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.ticketsControllerFindOne(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**Ticket**

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

# **ticketsControllerFindTickets**
> Array<Ticket> ticketsControllerFindTickets()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

const { status, data } = await apiInstance.ticketsControllerFindTickets();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Ticket>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of tickets for the board. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerFindTicketsByDriverId**
> object ticketsControllerFindTicketsByDriverId()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

const { status, data } = await apiInstance.ticketsControllerFindTicketsByDriverId();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**object**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List all tickets that belong to a driver. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerGetArrivalTimeCrane**
> ticketsControllerGetArrivalTimeCrane()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let ticketId: string; // (default to undefined)
let craneId: string; // (default to undefined)

const { status, data } = await apiInstance.ticketsControllerGetArrivalTimeCrane(
    ticketId,
    craneId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ticketId** | [**string**] |  | defaults to undefined|
| **craneId** | [**string**] |  | defaults to undefined|


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
|**200** | The arrival time. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerGetNearbyCranes**
> ticketsControllerGetNearbyCranes()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.ticketsControllerGetNearbyCranes(
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
|**200** | List of nearby cranes. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ticketsControllerRemove**
> ticketsControllerRemove()


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.ticketsControllerRemove(
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

# **ticketsControllerUpdate**
> Ticket ticketsControllerUpdate(body)


### Example

```typescript
import {
    TicketsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let id: string; // (default to undefined)
let body: object; //

const { status, data } = await apiInstance.ticketsControllerUpdate(
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

**Ticket**

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

# **ticketsControllerUpdateTicketStep**
> ticketsControllerUpdateTicketStep(updateTicketStepDto)


### Example

```typescript
import {
    TicketsApi,
    Configuration,
    UpdateTicketStepDto
} from './api';

const configuration = new Configuration();
const apiInstance = new TicketsApi(configuration);

let id: number; // (default to undefined)
let updateTicketStepDto: UpdateTicketStepDto; //

const { status, data } = await apiInstance.ticketsControllerUpdateTicketStep(
    id,
    updateTicketStepDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTicketStepDto** | **UpdateTicketStepDto**|  | |
| **id** | [**number**] |  | defaults to undefined|


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
|**200** | The ticket step has been successfully updated. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

