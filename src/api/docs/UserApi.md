# UserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bindUserWallet**](#binduserwallet) | **POST** /bind_user_wallet/{tg_id} | Bind User Wallet|
|[**collectReferralEarn**](#collectreferralearn) | **GET** /collect_referral_earn/{tg_id} | Collect Referral Earn|
|[**createReferralUser**](#createreferraluser) | **POST** /create_referral_user/{tg_id} | Create Referral User|
|[**getReferralLink**](#getreferrallink) | **POST** /get_referral_link/{tg_id} | Get Referral Link|
|[**getUserProgress**](#getuserprogress) | **GET** /get_user/{tg_id} | Get User Progress|
|[**saveProgress**](#saveprogress) | **POST** /save_progress/{tg_id} | Save Progress|

# **bindUserWallet**
> Error bindUserWallet(walletBody)


### Example

```typescript
import {
    UserApi,
    Configuration,
    WalletBody
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)
let walletBody: WalletBody; //Wallet body

const { status, data } = await apiInstance.bindUserWallet(
    tgId,
    walletBody
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **walletBody** | **WalletBody**| Wallet body | |
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
|**200** | Bind Wallet Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **collectReferralEarn**
> ReferralBalance collectReferralEarn()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.collectReferralEarn(
    tgId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**ReferralBalance**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Referral Balance Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createReferralUser**
> Error createReferralUser(referralLink)


### Example

```typescript
import {
    UserApi,
    Configuration,
    ReferralLink
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)
let referralLink: ReferralLink; //Referral Link Body

const { status, data } = await apiInstance.createReferralUser(
    tgId,
    referralLink
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **referralLink** | **ReferralLink**| Referral Link Body | |
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
|**200** | Referral Link Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getReferralLink**
> ReferralLink getReferralLink()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.getReferralLink(
    tgId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**ReferralLink**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Referral Link Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserProgress**
> User getUserProgress()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)

const { status, data } = await apiInstance.getUserProgress(
    tgId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tgId** | [**number**] | The tg ID of user | defaults to undefined|


### Return type

**User**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Get User Progress Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **saveProgress**
> Error saveProgress(tapTokenBody)


### Example

```typescript
import {
    UserApi,
    Configuration,
    TapTokenBody
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let tgId: number; //The tg ID of user (default to undefined)
let tapTokenBody: TapTokenBody; //Tap Token Body

const { status, data } = await apiInstance.saveProgress(
    tgId,
    tapTokenBody
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tapTokenBody** | **TapTokenBody**| Tap Token Body | |
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
|**200** | Save Progress Response |  -  |
|**400** | Bad request |  -  |
|**403** | Forbidden |  -  |
|**422** | Unprocessable Entity |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

