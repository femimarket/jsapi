# RevolutRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**revolut**](RevolutRouteApi.md#revolut) | **POST** /revolut |  |



## revolut

> Revolut revolut(amountCents, id, status, userId, credit, loaded, paymentUrl, revolutOrderId)



### Example

```ts
import {
  Configuration,
  RevolutRouteApi,
} from 'jsapi';
import type { RevolutRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RevolutRouteApi(config);

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
    revolutOrderId: revolutOrderId_example,
  } satisfies RevolutRequest;

  try {
    const data = await api.revolut(body);
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
| **revolutOrderId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Revolut**](Revolut.md)

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

