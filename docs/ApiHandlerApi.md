# ApiHandlerApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiHandler**](ApiHandlerApi.md#apihandler) | **POST** /api |  |



## apiHandler

> API apiHandler(aPI)



### Example

```ts
import {
  Configuration,
  ApiHandlerApi,
} from 'jsapi';
import type { ApiHandlerRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApiHandlerApi(config);

  const body = {
    // API
    aPI: ...,
  } satisfies ApiHandlerRequest;

  try {
    const data = await api.apiHandler(body);
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
| **aPI** | [API](API.md) |  | |

### Return type

[**API**](API.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Upload successful |  -  |
| **400** | Bad request |  -  |
| **402** | Payment required |  -  |
| **409** | Conflict |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

