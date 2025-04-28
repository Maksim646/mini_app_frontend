# NearApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**transitNear**](#transitnear) | **POST** /near_transaction | Transit Near|

# **transitNear**
> NearTransit transitNear(getNearBody)


### Example

```typescript
import {
    NearApi,
    Configuration,
    GetNearBody
} from './api';

const configuration = new Configuration();
const apiInstance = new NearApi(configuration);

let getNearBody: GetNearBody; //Get Near

const { status, data } = await apiInstance.transitNear(
    getNearBody
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **getNearBody** | **GetNearBody**| Get Near | |


### Return type

**NearTransit**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Transit Near Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

