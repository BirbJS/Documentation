---
layout: default
title: Birb
parent: Classes
has_children: false
has_toc: true
---

# Birb
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Birb(options)
```

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| options | BirbOptions |   | *none* |

# Properties
## baseApiUrl
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## guilds
**Type:** [GuildsManager](/classes/GuildsManager)

## intents
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** [Intents](/classes/Intents)

## options
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** BirbOptions

## ping
**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## users
**Type:** [UsersManager](/classes/UsersManager)

## ws
**Type:** [Websocket](/classes/Websocket)

# Methods
## clear()
**Returns:** void

## fly()
**Returns:** Promise<[Birb](/classes/Birb)>

## getToken()
**Returns:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## setToken(token)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| token | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | *none* |

**Returns:** [Birb](/classes/Birb)

## when(event)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| event | BirbEvent |   | *none* |

**Returns:** EventListener<BirbEvent, Function>

