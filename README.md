# JS Naming Conventions

## Language

Use English for defining your variables. The name should be short, concise, but at the same time descriptive enough, within reason. Horizontal space is less important than your code being immediately understandable by a new reader. Do not use abbreviations that are not common knowledge outside your company/business domain. Omiting letters or using contractions is also to be avoided.

```js
/* Bad */
const fornavn         // Different language
const r               // Meaningless - single letters do not tell much
const isPaginatable   // Incorrect grammatically
const cepos           // Unknown abbreviation
const custNum         // Deletes letters

/* Good */
const firstName
const customerNumber
```

## Casing

Generally you should pick one casing convention and stick to it. But since this is JS, the casing is circumstantial and should be applied as followed:
- `camelCase` - for defining variables
- `PascalCase` - for defining your classes, interfaces, records and type definitions
- `upper_snake_case` - for defining Enums and constants

This achieves a visual distinction on establishing the high level type a variable represents, improving readability.

```js
/* Bad */
const ReturnUrl = getReturnUrl()
const shoppingItem = <ShoppingCard />
const defaultPageSize = 100

/* Good */
const returnUrl = getReturnUrl()
const ShoppingItem = <ShoppingCard />
const DEFAULT_PAGE_SIZE = 100
```

## Naming structure

When converting English phrases into code there are many ways of doing it. Acronyms and specific words such as "iOS" make things more tricky, when trying to define a deterministic structure.

For this there are a few steps:

1. Split the prose form on spaces
2. Lowercase everything
3. Apply the [casing convention](#casing) based on the type of the variable

> **Note:** Some words such as "iOS" are able to break these conventions


| Prose form             | Accepted form        | Incorrect example    |
| ---------------------- | -------------------- | -------------------- |
| `GraphQL Request`      | `graphqlRequest`     | `graphQLRequest`     |
| `XHR Request`          | `xhrRequest`         | `xHRRequest`         |
| `Default Number`       | `DEFAULT_NUMBER`     | `defaultNumber`      |
| `Shopping Cart Button` | `ShoppingCartButton` | `shoppingCartButton` |


### Composable prose form

In order for naming to be meaningful, the prose form needs to follow a pattern.

## Filenames

Filenames should **always** match their default export.
When there is not default export, the file should default to `camelCase`.

## Imports

