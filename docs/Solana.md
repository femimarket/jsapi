
# Solana


## Properties

Name | Type
------------ | -------------
`amountCents` | number
`credit` | number
`id` | string
`loaded` | boolean
`pubkey` | string
`quotedOutUnits` | number
`requestId` | string
`signature` | string
`signedTx` | string
`status` | [Status](Status.md)
`unsignedTx` | string
`userId` | string

## Example

```typescript
import type { Solana } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "amountCents": null,
  "credit": null,
  "id": null,
  "loaded": null,
  "pubkey": null,
  "quotedOutUnits": null,
  "requestId": null,
  "signature": null,
  "signedTx": null,
  "status": null,
  "unsignedTx": null,
  "userId": null,
} satisfies Solana

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Solana
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


