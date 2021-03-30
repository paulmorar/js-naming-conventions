# JS Naming Conventions

## Language

Use English for defining your variables. The name should be descriptive enough, within reason. Horizontal space is less important than your code being immediately understandable by a new reader. Do not use abbreviations that are not common knowledge outside your company/business domain.

```js
/* Bad */
const fornavn // Different language
const r       // Meaningless - single letters do not tell much
const cepos   // Unknown abbreviation
const custNum // Deletes letters

/* Good */
const firstName
const customerNumber
```

## Casing

Generally you should pick one casing convention and stick to it. But since this is JS, the casing is circumstantial and should be applied as followed:
`camelCase` - for defining variables
`PascalCase` - for defining your classes and components
