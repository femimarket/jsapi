
# PayProvider

Which app store a purchase came from. Selects the verification path in `pre`. Schema name `PayProvider` to avoid clashing with the unrelated `provider::Provider` in the OpenAPI components.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { PayProvider } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
} satisfies PayProvider

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayProvider
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


