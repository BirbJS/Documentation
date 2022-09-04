---
layout: default
title: SystemChannelFlags
parent: Classes
has_children: false
has_toc: true
---

# SystemChannelFlags
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new SystemChannelFlags(bits?)
```

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| bits? | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| bigint |   | *none* |

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
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** [SystemChannelFlags](/classes/SystemChannelFlags)

## clone()
**Returns:** [SystemChannelFlags](/classes/SystemChannelFlags)

## convert(flags)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | BitResolvable<SUPPRESS_JOIN_NOTIFICATIONS \| SUPPRESS_PREMIUM_SUBSCRIPTIONS \| SUPPRESS_GUILD_REMINDER_NOTIFICATIONS \| SUPPRESS_JOIN_NOTIFICATION_REPLIES> \| *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** bigint

## has(flags)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isEmpty()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isLocked()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## remove(flags)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** [SystemChannelFlags](/classes/SystemChannelFlags)

## set(flags)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** [SystemChannelFlags](/classes/SystemChannelFlags)

## toArray()
**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## toBigInt()
**Returns:** bigint

