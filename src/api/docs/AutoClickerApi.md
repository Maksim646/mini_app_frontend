# AutoClickerApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**startAutoClicker**](#startautoclicker) | **POST** /start_auto_clicker/{tg_id} | Start Auto Clicker|
|[**stopAutoClicker**](#stopautoclicker) | **POST** /stop_auto_clicker/{tg_id} | Stop Auto Clicker|

# **startAutoClicker**
> Error startAutoClicker()


### Example

```typescript
import {
    AutoClickerApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AutoClickerApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.startAutoClicker(
    tgId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**Error**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Save Progress Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **stopAutoClicker**
> Error stopAutoClicker()


### Example

```typescript
import {
    AutoClickerApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AutoClickerApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.stopAutoClicker(
    tgId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**Error**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Save Progress Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

