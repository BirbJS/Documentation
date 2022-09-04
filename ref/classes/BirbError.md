---
layout: default
title: BirbError
parent: Classes
has_children: false
has_toc: true
---

# BirbError
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new BirbError(message)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

# Properties
## cause
**Type:** unknown

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

