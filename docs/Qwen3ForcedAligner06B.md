
# Qwen3ForcedAligner06B


## Properties

Name | Type
------------ | -------------
`audio` | string
`characters` | [Array&lt;CharacterAlignment&gt;](CharacterAlignment.md)
`lyrics` | string
`type` | string
`words` | [Array&lt;WordAlignment&gt;](WordAlignment.md)

## Example

```typescript
import type { Qwen3ForcedAligner06B } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "audio": null,
  "characters": null,
  "lyrics": null,
  "type": null,
  "words": null,
} satisfies Qwen3ForcedAligner06B

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Qwen3ForcedAligner06B
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


