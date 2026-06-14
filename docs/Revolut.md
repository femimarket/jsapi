
# Revolut


## Properties

Name | Type
------------ | -------------
`amountCents` | number
`credit` | number
`id` | string
`loaded` | boolean
`paymentUrl` | string
`revolutOrderId` | string
`status` | [Status](Status.md)
`userId` | string

## Example

```typescript
import type { Revolut } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "amountCents": null,
  "credit": null,
  "id": null,
  "loaded": null,
  "paymentUrl": null,
  "revolutOrderId": null,
  "status": null,
  "userId": null,
} satisfies Revolut

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Revolut
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


