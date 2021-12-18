---
layout: default
title: Request
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# Request
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Request(client, method, path, body?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) |   | false | *none* |
| method | HTTPMethod |   | false | *none* |
| path | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |
| body | any |   | true | *none* |

# Properties
## body
**Type:** any

## client
**Type:** [Client](/ref/classes/Client)

## method
**Type:** HTTPMethod

## reason
**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## response
**Type:** any

## upload
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## url
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## make(files?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| files | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** Promise<any>

