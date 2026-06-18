
# ApplePay


## Properties

Name | Type
------------ | -------------
`credit` | number
`currency` | string
`jws` | string
`loaded` | boolean
`price` | number
`productId` | string
`transactionId` | string
`type` | string

## Example

```typescript
import type { ApplePay } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "credit": null,
  "currency": null,
  "jws": null,
  "loaded": null,
  "price": null,
  "productId": null,
  "transactionId": null,
  "type": null,
} satisfies ApplePay

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApplePay
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


