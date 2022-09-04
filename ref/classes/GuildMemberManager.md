---
layout: default
title: GuildMemberManager
parent: Classes
has_children: false
has_toc: true
---

# GuildMemberManager
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildMemberManager(client, guild)
```

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| client | [Birb](/classes/Birb) |   | *none* |
| guild | [Guild](/classes/Guild) |   | *none* |

# Properties
## cache
**Type:** Cache<*[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*, [GuildMember](/classes/GuildMember)>

## client
**Type:** [Birb](/classes/Birb)

## guild
**Type:** [Guild](/classes/Guild)

# Methods
## fetch(target)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| target | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* \| [GuildMember](/classes/GuildMember) |   | *none* |

**Returns:** Promise<*[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| [GuildMember](/classes/GuildMember)>

## resolve(target)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| target | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* \| [GuildMember](/classes/GuildMember) |   | *none* |

**Returns:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| [GuildMember](/classes/GuildMember)

## total()
**Returns:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

