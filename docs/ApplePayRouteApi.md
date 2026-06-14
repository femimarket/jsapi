# ApplePayRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**applePay**](ApplePayRouteApi.md#applepay) | **POST** /apple_pay |  |



## applePay

> ApplePay applePay(credit, currency, id, jws, loaded, price, productId, status, transactionId, userId)



### Example

```ts
import {
  Configuration,
  ApplePayRouteApi,
} from 'jsapi';
import type { ApplePayRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplePayRouteApi(config);

  const body = {
    // number
    credit: 789,
    // string
    currency: currency_example,
    // string | uuid v7
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    jws: jws_example,
    // boolean
    loaded: true,
    // number
    price: 789,
    // string
    productId: productId_example,
    // ApplePayStatus
    status: ...,
    // string
    transactionId: transactionId_example,
    // string
    userId: userId_example,
  } satisfies ApplePayRequest;

  try {
    const data = await api.applePay(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **credit** | `number` |  | [Defaults to `undefined`] |
| **currency** | `string` |  | [Defaults to `undefined`] |
| **id** | `string` | uuid v7 | [Defaults to `undefined`] |
| **jws** | `string` |  | [Defaults to `undefined`] |
| **loaded** | `boolean` |  | [Defaults to `undefined`] |
| **price** | `number` |  | [Defaults to `undefined`] |
| **productId** | `string` |  | [Defaults to `undefined`] |
| **status** | `ApplePayStatus` |  | [Defaults to `undefined`] [Enum: Pending, Completed, Failed] |
| **transactionId** | `string` |  | [Defaults to `undefined`] |
| **userId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ApplePay**](ApplePay.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Upload successful |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

