
# Model


## Properties

Name | Type
------------ | -------------
`amountCents` | number
`credit` | number
`id` | string
`loaded` | boolean
`paymentUrl` | string
`status` | [Status](Status.md)
`stripePaymentIntentId` | string
`stripeSessionId` | string
`userId` | string

## Example

```typescript
import type { Model } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "amountCents": null,
  "credit": null,
  "id": null,
  "loaded": null,
  "paymentUrl": null,
  "status": null,
  "stripePaymentIntentId": null,
  "stripeSessionId": null,
  "userId": null,
} satisfies Model

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Model
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


