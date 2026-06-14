
# ApiPay

default values

## Properties

Name | Type
------------ | -------------
`currency` | string
`id` | string
`jws` | string
`loaded` | boolean
`orderId` | string
`packageName` | string
`price` | number
`productId` | string
`provider` | [ApiPayProvider](ApiPayProvider.md)
`refId` | string
`userId` | string

## Example

```typescript
import type { ApiPay } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "currency": null,
  "id": null,
  "jws": null,
  "loaded": null,
  "orderId": null,
  "packageName": null,
  "price": null,
  "productId": null,
  "provider": null,
  "refId": null,
  "userId": null,
} satisfies ApiPay

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApiPay
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


