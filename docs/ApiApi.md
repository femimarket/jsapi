# ApiApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiHandler**](ApiApi.md#apihandler) | **POST** /api |  |
| [**mediaGate**](ApiApi.md#mediagate) | **GET** /{file} | Auth + per-GB debit gate in front of the &#x60;_upload&#x60; ServeDir on femi.market.   - not a media file → pass through (static site, app data, 404), free   - media file that isn\&#39;t a real file in &#x60;_upload&#x60; → pass through, free   - media file in &#x60;_upload&#x60; → require Bearer, charge &#x60;size × pricing.gb&#x60;,     record a debit in the astc ledger, then let ServeDir stream the bytes. The gate only authorizes/charges; ServeDir still does the actual file streaming (range requests, mime, etc.). |



## apiHandler

> API apiHandler(aPI)



### Example

```ts
import {
  Configuration,
  ApiApi,
} from 'jsapi';
import type { ApiHandlerRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApiApi(config);

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


## mediaGate

> Array&lt;number&gt; mediaGate(file)

Auth + per-GB debit gate in front of the &#x60;_upload&#x60; ServeDir on femi.market.   - not a media file → pass through (static site, app data, 404), free   - media file that isn\&#39;t a real file in &#x60;_upload&#x60; → pass through, free   - media file in &#x60;_upload&#x60; → require Bearer, charge &#x60;size × pricing.gb&#x60;,     record a debit in the astc ledger, then let ServeDir stream the bytes. The gate only authorizes/charges; ServeDir still does the actual file streaming (range requests, mime, etc.).

&#x60;#[utoipa::path]&#x60; here is doc-only — the fn runs as &#x60;from_fn&#x60; middleware, not a route handler, but the attribute still emits the spec entry so the generated clients get a typed &#x60;downloadMedia(file)&#x60;. &#x60;servers(...)&#x60; pins it to femi.market (the global server is api.earnfemi.com); &#x60;Request&#x60;/&#x60;Next&#x60; args aren\&#39;t documentable extractors so utoipa ignores them and uses the explicit &#x60;params&#x60;.

### Example

```ts
import {
  Configuration,
  ApiApi,
} from 'jsapi';
import type { MediaGateRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApiApi(config);

  const body = {
    // string | media filename in _upload
    file: file_example,
  } satisfies MediaGateRequest;

  try {
    const data = await api.mediaGate(body);
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
| **file** | `string` | media filename in _upload | [Defaults to `undefined`] |

### Return type

**Array<number>**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/octet-stream`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | media bytes |  -  |
| **401** | missing/invalid bearer |  -  |
| **402** | insufficient credits |  -  |
| **404** | not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

