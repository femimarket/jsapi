# WiseRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**wise**](WiseRouteApi.md#wise) | **POST** /wise |  |



## wise

> Wise wise(amountCents, currency, id, reference, status, userId, credit, loaded, wiseCreditId)



### Example

```ts
import {
  Configuration,
  WiseRouteApi,
} from 'jsapi';
import type { WiseRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WiseRouteApi(config);

  const body = {
    // number
    amountCents: 789,
    // string
    currency: currency_example,
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    reference: reference_example,
    // Status
    status: ...,
    // string
    userId: userId_example,
    // number (optional)
    credit: 789,
    // boolean (optional)
    loaded: true,
    // string (optional)
    wiseCreditId: wiseCreditId_example,
  } satisfies WiseRequest;

  try {
    const data = await api.wise(body);
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
| **currency** | `string` |  | [Defaults to `undefined`] |
| **id** | `string` |  | [Defaults to `undefined`] |
| **reference** | `string` |  | [Defaults to `undefined`] |
| **status** | `Status` |  | [Defaults to `undefined`] [Enum: 1, 2, 3] |
| **userId** | `string` |  | [Defaults to `undefined`] |
| **credit** | `number` |  | [Optional] [Defaults to `undefined`] |
| **loaded** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **wiseCreditId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Wise**](Wise.md)

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

