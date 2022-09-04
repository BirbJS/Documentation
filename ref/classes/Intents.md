---
layout: default
title: Intents
parent: Classes
has_children: false
has_toc: true
---

# Intents
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Intents(bits?)
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

**Returns:** [Intents](/classes/Intents)

## clone()
**Returns:** [Intents](/classes/Intents)

## convert(flags)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | BitResolvable<GUILDS \| GUILD_MEMBERS \| GUILD_BANS \| GUILD_EMOJIS_AND_STICKERS \| GUILD_INTEGRATIONS \| GUILD_WEBHOOKS \| GUILD_INVITES \| GUILD_VOICE_STATES \| GUILD_PRESENCES \| GUILD_MESSAGES \| GUILD_MESSAGE_REACTIONS \| GUILD_MESSAGE_TYPING \| DIRECT_MESSAGES \| DIRECT_MESSAGE_REACTIONS \| DIRECT_MESSAGE_TYPING \| MESSAGE_CONTENT \| GUILD_SCHEDULED_EVENTS \| AUTO_MODERATION_CONFIGURATION \| AUTO_MODERATION_EXECUTION> \| *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

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

**Returns:** [Intents](/classes/Intents)

## set(flags)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** [Intents](/classes/Intents)

## toArray()
**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## toBigInt()
**Returns:** bigint

