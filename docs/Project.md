
# Project


## Properties

Name | Type
------------ | -------------
`about` | string
`audio` | string
`audioLines` | [Array&lt;AudioLine&gt;](AudioLine.md)
`faqs` | [Array&lt;Faq&gt;](Faq.md)
`genre` | string
`id` | string
`playlist` | string
`seasons` | [Array&lt;Season&gt;](Season.md)
`summary` | string
`userId` | string

## Example

```typescript
import type { Project } from 'jsapi'

// TODO: Update the object below with actual values
const example = {
  "about": null,
  "audio": null,
  "audioLines": null,
  "faqs": null,
  "genre": null,
  "id": null,
  "playlist": null,
  "seasons": null,
  "summary": null,
  "userId": null,
} satisfies Project

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Project
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


