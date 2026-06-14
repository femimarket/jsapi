# SolanaRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**solana**](SolanaRouteApi.md#solana) | **POST** /solana |  |



## solana

> Solana solana(amountCents, id, pubkey, status, userId, credit, loaded, quotedOutUnits, requestId, signature, signedTx, unsignedTx)



### Example

```ts
import {
  Configuration,
  SolanaRouteApi,
} from 'jsapi';
import type { SolanaRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SolanaRouteApi(config);

  const body = {
    // number
    amountCents: 789,
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    pubkey: pubkey_example,
    // Status
    status: ...,
    // string
    userId: userId_example,
    // number (optional)
    credit: 789,
    // boolean (optional)
    loaded: true,
    // number (optional)
    quotedOutUnits: 789,
    // string (optional)
    requestId: requestId_example,
    // string (optional)
    signature: signature_example,
    // string (optional)
    signedTx: signedTx_example,
    // string (optional)
    unsignedTx: unsignedTx_example,
  } satisfies SolanaRequest;

  try {
    const data = await api.solana(body);
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
| **pubkey** | `string` |  | [Defaults to `undefined`] |
| **status** | `Status` |  | [Defaults to `undefined`] [Enum: 1, 2, 3] |
| **userId** | `string` |  | [Defaults to `undefined`] |
| **credit** | `number` |  | [Optional] [Defaults to `undefined`] |
| **loaded** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **quotedOutUnits** | `number` |  | [Optional] [Defaults to `undefined`] |
| **requestId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **signature** | `string` |  | [Optional] [Defaults to `undefined`] |
| **signedTx** | `string` |  | [Optional] [Defaults to `undefined`] |
| **unsignedTx** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Solana**](Solana.md)

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

