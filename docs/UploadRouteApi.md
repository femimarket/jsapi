# UploadRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**upload**](UploadRouteApi.md#upload) | **POST** /upload |  |



## upload

> Upload upload(credit, file, id, userId)



### Example

```ts
import {
  Configuration,
  UploadRouteApi,
} from 'jsapi';
import type { UploadRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UploadRouteApi(config);

  const body = {
    // number
    credit: 789,
    // string
    file: file_example,
    // string | uuid v7
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    userId: userId_example,
  } satisfies UploadRequest;

  try {
    const data = await api.upload(body);
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
| **file** | `string` |  | [Defaults to `undefined`] |
| **id** | `string` | uuid v7 | [Defaults to `undefined`] |
| **userId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Upload**](Upload.md)

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

