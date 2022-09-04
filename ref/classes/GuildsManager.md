---
layout: default
title: GuildsManager
parent: Classes
has_children: false
has_toc: true
---

# GuildsManager
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildsManager(client)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |

# Properties
## cache
**Type:** Cache<*[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*, [Guild](/classes/Guild)>

## client
**Type:** [Birb](/classes/Birb)

## unavailableCache
**Type:** Cache<*[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*, [GuildPartial](/classes/GuildPartial)>

# Methods
## fetch(target)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| target | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* \| [GuildPartial](/classes/GuildPartial) \| [Guild](/classes/Guild) |   | false | *none* |

**Returns:** Promise<*[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| [Guild](/classes/Guild)>

## resolve(target)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| target | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* \| [GuildPartial](/classes/GuildPartial) \| [Guild](/classes/Guild) |   | false | *none* |

**Returns:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| [GuildPartial](/classes/GuildPartial) \| [Guild](/classes/Guild)

## total()
**Returns:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

