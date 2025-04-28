# CardsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getUserCards**](#getusercards) | **POST** /get_user_cards/{tg_id} | Get User Cards|
|[**updateUserCard**](#updateusercard) | **POST** /update_user_card/{tg_id} | Update User Card|

# **getUserCards**
> CardsBody getUserCards()


### Example

```typescript
import {
    CardsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CardsApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.getUserCards(
    tgId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**CardsBody**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Get User Cards Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateUserCard**
> CardBody updateUserCard(cardUpdateBody)


### Example

```typescript
import {
    CardsApi,
    Configuration,
    CardUpdateBody
} from './api';

const configuration = new Configuration();
const apiInstance = new CardsApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)
let cardUpdateBody: CardUpdateBody; //Card Update Body

const { status, data } = await apiInstance.updateUserCard(
    tgId,
    cardUpdateBody
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cardUpdateBody** | **CardUpdateBody**| Card Update Body | |
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**CardBody**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Update Card Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

