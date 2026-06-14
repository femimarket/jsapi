
# LyricSync


## Properties

Name | Type
------------ | -------------
`audio` | string
`characters` | [Array&lt;CharacterAlignment&gt;](CharacterAlignment.md)
`credit` | number
`id` | string
`loss` | number
`lyrics` | string
`userId` | string
`words` | [Array&lt;WordAlignment&gt;](WordAlignment.md)

## Example

```typescript
import type { LyricSync } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "audio": null,
  "characters": null,
  "credit": null,
  "id": null,
  "loss": null,
  "lyrics": null,
  "userId": null,
  "words": null,
} satisfies LyricSync

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LyricSync
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


