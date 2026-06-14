# LyricSyncRouteApi

All URIs are relative to *https://api.earnfemi.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**lyricSync**](LyricSyncRouteApi.md#lyricsync) | **POST** /lyric_sync |  |



## lyricSync

> LyricSync lyricSync(audio, id, lyrics, characters, credit, loss, userId, words)



### Example

```ts
import {
  Configuration,
  LyricSyncRouteApi,
} from 'jsapi';
import type { LyricSyncRequest } from 'jsapi';

async function example() {
  console.log("🚀 Testing jsapi SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LyricSyncRouteApi(config);

  const body = {
    // string
    audio: audio_example,
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    lyrics: lyrics_example,
    // Array<CharacterAlignment> (optional)
    characters: ...,
    // number (optional)
    credit: 789,
    // number (optional)
    loss: 1.2,
    // string (optional)
    userId: userId_example,
    // Array<WordAlignment> (optional)
    words: ...,
  } satisfies LyricSyncRequest;

  try {
    const data = await api.lyricSync(body);
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
| **audio** | `string` |  | [Defaults to `undefined`] |
| **id** | `string` |  | [Defaults to `undefined`] |
| **lyrics** | `string` |  | [Defaults to `undefined`] |
| **characters** | `Array<CharacterAlignment>` |  | [Optional] |
| **credit** | `number` |  | [Optional] [Defaults to `undefined`] |
| **loss** | `number` |  | [Optional] [Defaults to `undefined`] |
| **userId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **words** | `Array<WordAlignment>` |  | [Optional] |

### Return type

[**LyricSync**](LyricSync.md)

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

