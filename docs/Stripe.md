
# Stripe


## Properties

Name | Type
------------ | -------------
`amountCents` | number
`credit` | number
`loaded` | boolean
`paymentUrl` | string
`stripePaymentIntentId` | string
`stripeSessionId` | string
`type` | string

## Example

```typescript
import type { Stripe } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "amountCents": null,
  "credit": null,
  "loaded": null,
  "paymentUrl": null,
  "stripePaymentIntentId": null,
  "stripeSessionId": null,
  "type": null,
} satisfies Stripe

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Stripe
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


