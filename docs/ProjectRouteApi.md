# ProjectRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**project**](ProjectRouteApi.md#project) | **POST** /project |  |



## project

> Project project(about, audio, audioLines, faqs, genre, id, playlist, seasons, summary, userId)



### Example

```ts
import {
  Configuration,
  ProjectRouteApi,
} from 'jsapi';
import type { ProjectRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProjectRouteApi(config);

  const body = {
    // string
    about: about_example,
    // string
    audio: audio_example,
    // Array<AudioLine>
    audioLines: ...,
    // Array<Faq>
    faqs: ...,
    // string
    genre: genre_example,
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    playlist: playlist_example,
    // Array<Season>
    seasons: ...,
    // string
    summary: summary_example,
    // string
    userId: userId_example,
  } satisfies ProjectRequest;

  try {
    const data = await api.project(body);
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
| **about** | `string` |  | [Defaults to `undefined`] |
| **audio** | `string` |  | [Defaults to `undefined`] |
| **audioLines** | `Array<AudioLine>` |  | |
| **faqs** | `Array<Faq>` |  | |
| **genre** | `string` |  | [Defaults to `undefined`] |
| **id** | `string` |  | [Defaults to `undefined`] |
| **playlist** | `string` |  | [Defaults to `undefined`] |
| **seasons** | `Array<Season>` |  | |
| **summary** | `string` |  | [Defaults to `undefined`] |
| **userId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Project**](Project.md)

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

