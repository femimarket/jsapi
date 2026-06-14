# StripeRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**stripe**](StripeRouteApi.md#stripe) | **POST** /stripe |  |



## stripe

> Model stripe(amountCents, id, status, userId, credit, loaded, paymentUrl, stripePaymentIntentId, stripeSessionId)



### Example

```ts
import {
  Configuration,
  StripeRouteApi,
} from 'jsapi';
import type { StripeRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StripeRouteApi(config);

  const body = {
    // number
    amountCents: 789,
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // Status
    status: ...,
    // string
    userId: userId_example,
    // number (optional)
    credit: 789,
    // boolean (optional)
    loaded: true,
    // string (optional)
    paymentUrl: paymentUrl_example,
    // string (optional)
    stripePaymentIntentId: stripePaymentIntentId_example,
    // string (optional)
    stripeSessionId: stripeSessionId_example,
  } satisfies StripeRequest;

  try {
    const data = await api.stripe(body);
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
| **amountCents** | `number` |  | [Defaults to `undefined`] |
| **id** | `string` |  | [Defaults to `undefined`] |
| **status** | `Status` |  | [Defaults to `undefined`] [Enum: 1, 2, 3] |
| **userId** | `string` |  | [Defaults to `undefined`] |
| **credit** | `number` |  | [Optional] [Defaults to `undefined`] |
| **loaded** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **paymentUrl** | `string` |  | [Optional] [Defaults to `undefined`] |
| **stripePaymentIntentId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **stripeSessionId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Model**](Model.md)

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

