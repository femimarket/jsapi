
# GooglePay


## Properties

Name | Type
------------ | -------------
`credit` | number
`loaded` | boolean
`orderId` | string
`packageName` | string
`productId` | string
`purchaseToken` | string
`type` | string

## Example

```typescript
import type { GooglePay } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "credit": null,
  "loaded": null,
  "orderId": null,
  "packageName": null,
  "productId": null,
  "purchaseToken": null,
  "type": null,
} satisfies GooglePay

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GooglePay
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


