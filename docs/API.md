
# API

default values

## Properties

Name | Type
------------ | -------------
`action` | [ApiAction](ApiAction.md)
`credit` | number
`id` | string
`status` | [ApiStatus](ApiStatus.md)
`userId` | string

## Example

```typescript
import type { API } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "action": null,
  "credit": null,
  "id": null,
  "status": null,
  "userId": null,
} satisfies API

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as API
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


