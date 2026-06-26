
# ApiAction


## Properties

Name | Type
------------ | -------------
`description` | string
`type` | string
`falRequestId` | string
`file` | string
`prompt` | string
`audio` | string
`comfyRequestId` | string
`image` | string
`image2` | string
`messages` | [Array&lt;ApiChatMessage&gt;](ApiChatMessage.md)
`credit` | number
`currency` | string
`jws` | string
`loaded` | boolean
`price` | number
`productId` | string
`transactionId` | string
`orderId` | string
`packageName` | string
`purchaseToken` | string
`lyrics` | string

## Example

```typescript
import type { ApiAction } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "description": null,
  "type": null,
  "falRequestId": null,
  "file": null,
  "prompt": null,
  "audio": null,
  "comfyRequestId": null,
  "image": null,
  "image2": null,
  "messages": null,
  "credit": null,
  "currency": null,
  "jws": null,
  "loaded": null,
  "price": null,
  "productId": null,
  "transactionId": null,
  "orderId": null,
  "packageName": null,
  "purchaseToken": null,
  "lyrics": null,
} satisfies ApiAction

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApiAction
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


