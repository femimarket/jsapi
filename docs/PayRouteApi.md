# PayRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**pay**](PayRouteApi.md#pay) | **POST** /pay |  |



## pay

> Pay pay(id, provider, userId, credit, currency, jws, loaded, orderId, packageName, price, productId, refId, status)



### Example

```ts
import {
  Configuration,
  PayRouteApi,
} from 'jsapi';
import type { PayRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PayRouteApi(config);

  const body = {
    // string | uuid v7
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // PayProvider | Selects the verification path: Apple App Store vs Google Play.
    provider: ...,
    // string
    userId: userId_example,
    // number (optional)
    credit: 789,
    // string (optional)
    currency: currency_example,
    // string | Signed transaction JWS from StoreKit; the input to Apple verification. (optional)
    jws: jws_example,
    // boolean (optional)
    loaded: true,
    // string | Google\\\'s per-purchase `orderId`, returned by the Play Developer API (not the client). Not used for dedup — `ref_id` is — because promo-code purchases may have no `orderId`. (optional)
    orderId: orderId_example,
    // string (optional)
    packageName: packageName_example,
    // number (optional)
    price: 789,
    // string (optional)
    productId: productId_example,
    // string | Globally-unique purchase id, used as the idempotency key for both stores. Apple: the `transactionId`, extracted server-side from the verified JWS   (empty on the incoming request — the server fills it in). Google: the `purchaseToken`, sent by the client. It is both the input to   Play Developer API verification and the idempotency key. (optional)
    refId: refId_example,
    // PayStatus (optional)
    status: ...,
  } satisfies PayRequest;

  try {
    const data = await api.pay(body);
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
| **id** | `string` | uuid v7 | [Defaults to `undefined`] |
| **provider** | `PayProvider` | Selects the verification path: Apple App Store vs Google Play. | [Defaults to `undefined`] [Enum: Apple, Google] |
| **userId** | `string` |  | [Defaults to `undefined`] |
| **credit** | `number` |  | [Optional] [Defaults to `undefined`] |
| **currency** | `string` |  | [Optional] [Defaults to `undefined`] |
| **jws** | `string` | Signed transaction JWS from StoreKit; the input to Apple verification. | [Optional] [Defaults to `undefined`] |
| **loaded** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **orderId** | `string` | Google\\\&#39;s per-purchase &#x60;orderId&#x60;, returned by the Play Developer API (not the client). Not used for dedup — &#x60;ref_id&#x60; is — because promo-code purchases may have no &#x60;orderId&#x60;. | [Optional] [Defaults to `undefined`] |
| **packageName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **price** | `number` |  | [Optional] [Defaults to `undefined`] |
| **productId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **refId** | `string` | Globally-unique purchase id, used as the idempotency key for both stores. Apple: the &#x60;transactionId&#x60;, extracted server-side from the verified JWS   (empty on the incoming request — the server fills it in). Google: the &#x60;purchaseToken&#x60;, sent by the client. It is both the input to   Play Developer API verification and the idempotency key. | [Optional] [Defaults to `undefined`] |
| **status** | `PayStatus` |  | [Optional] [Defaults to `undefined`] [Enum: Pending, Completed, Failed] |

### Return type

[**Pay**](Pay.md)

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

