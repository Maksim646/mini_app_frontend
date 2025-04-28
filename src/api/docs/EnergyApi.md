# EnergyApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**startEnergyOffline**](#startenergyoffline) | **POST** /start_energy_collect/{tg_id} | Start Energy Offline|
|[**stopEnergyOffline**](#stopenergyoffline) | **POST** /stop_energy_collect/{tg_id} | Stop Energy Offline|

# **startEnergyOffline**
> Error startEnergyOffline(startEnergyCollectBody)


### Example

```typescript
import {
    EnergyApi,
    Configuration,
    StartEnergyCollectBody
} from './api';

const configuration = new Configuration();
const apiInstance = new EnergyApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)
let startEnergyCollectBody: StartEnergyCollectBody; //Start Energy Collect Body

const { status, data } = await apiInstance.startEnergyOffline(
    tgId,
    startEnergyCollectBody
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **startEnergyCollectBody** | **StartEnergyCollectBody**| Start Energy Collect Body | |
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**Error**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Start Collect Energy Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **stopEnergyOffline**
> Error stopEnergyOffline()


### Example

```typescript
import {
    EnergyApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EnergyApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.stopEnergyOffline(
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
|**200** | Stop Collect Energy Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

