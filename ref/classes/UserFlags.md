---
layout: default
title: UserFlags
parent: Classes
has_children: false
has_toc: true
---

# UserFlags
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new UserFlags(bits?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| bits | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| bigint |   | true | *none* |

# Properties
## bits
**Type:** bigint

## FLAGS
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

# Methods
## add(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** [UserFlags](/classes/UserFlags)

## clone()
**Returns:** [UserFlags](/classes/UserFlags)

## convert(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | BitResolvable<STAFF \| PARTNER \| HYPESQUAD \| BUG_HUNTER_LEVEL_1 \| HYPESQUAD_ONLINE_HOUSE_BRAVERY \| HYPESQUAD_ONLINE_HOUSE_BRILLIANCE \| HYPESQUAD_ONLINE_HOUSE_BALANCE \| NITRO_EARLY_SUPPORTER \| TEAM_PSEUDO_USER \| BUG_HUNTER_LEVEL_2 \| VERIFIED_BOT \| VERIFIED_BOT_DEVELOPER \| CERTIFIED_MODERATOR \| BOT_HTTP_INTERACTIONS> \| *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** bigint

## has(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isEmpty()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isLocked()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## remove(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** [UserFlags](/classes/UserFlags)

## set(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** [UserFlags](/classes/UserFlags)

## toArray()
**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## toBigInt()
**Returns:** bigint

