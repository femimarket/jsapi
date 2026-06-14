# ApiKeyRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiKey**](ApiKeyRouteApi.md#apikey) | **POST** /api_key |  |



## apiKey

> ApiKey apiKey(id, userId, key)



### Example

```ts
import {
  Configuration,
  ApiKeyRouteApi,
} from 'jsapi';
import type { ApiKeyRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApiKeyRouteApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    userId: userId_example,
    // string (optional)
    key: key_example,
  } satisfies ApiKeyRequest;

  try {
    const data = await api.apiKey(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |
| **userId** | `string` |  | [Defaults to `undefined`] |
| **key** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**ApiKey**](ApiKey.md)

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

