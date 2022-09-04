---
layout: default
title: BirbAPIError
parent: Classes
has_children: false
has_toc: true
---

# BirbAPIError
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new BirbAPIError(message, request, status, json?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |
| request | APIEndpoint<any, any, any> |   | false | *none* |
| status | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | false | *none* |
| json | any |   | true | *none* |

# Properties
## body
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** any

## cause
**Type:** unknown

## endpoint
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## headers
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## json
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** any

## message
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## name
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## package
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** birb

## stack
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## status
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## prepareStackTrace
{: .d-inline-block }

STATIC
{: .label .label-blue }

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## stackTraceLimit
{: .d-inline-block }

STATIC
{: .label .label-blue }

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

# Methods
## captureStackTrace(targetObject, constructorOpt?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| targetObject | *[object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/object)* |   | false | *none* |
| constructorOpt | Function |   | true | *none* |

**Returns:** void

