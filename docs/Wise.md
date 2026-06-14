
# Wise


## Properties

Name | Type
------------ | -------------
`amountCents` | number
`credit` | number
`currency` | string
`id` | string
`loaded` | boolean
`reference` | string
`status` | [Status](Status.md)
`userId` | string
`wiseCreditId` | string

## Example

```typescript
import type { Wise } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "amountCents": null,
  "credit": null,
  "currency": null,
  "id": null,
  "loaded": null,
  "reference": null,
  "status": null,
  "userId": null,
  "wiseCreditId": null,
} satisfies Wise

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Wise
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


