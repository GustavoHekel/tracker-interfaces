# PaymentsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**paymentsControllerFindAllPaymentTypes**](#paymentscontrollerfindallpaymenttypes) | **GET** /payments/types | List all payment types|

# **paymentsControllerFindAllPaymentTypes**
> Array<PaymentType> paymentsControllerFindAllPaymentTypes()


### Example

```typescript
import {
    PaymentsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PaymentsApi(configuration);

const { status, data } = await apiInstance.paymentsControllerFindAllPaymentTypes();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<PaymentType>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of all payment types |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

