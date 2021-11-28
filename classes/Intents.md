---
layout: default
title: Intents
parent: Classes
has_toc: true
---

# Intents
The Discord API uses intents to determine what events should be sent to connected clients. Intents are now **required** when connecting. You may use `Intents.FLAGS.ALL` to enable all intents, and `Intents.FLAGS.NOT_PRIVILEGED` to enable all intents that don't require approval (for verified bots).

### Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Constructor
`new Intents(...flags)`

| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| ...flags               | The intents to use    | Number (or from Intents.FLAGS)   | false    | none        |

# Properties

## flags
The intents that are enabled.

**Type:** Number (from Intents.FLAGS)

## Intents.FLAGS
{: .d-inline-block }

STATIC
{: .label .label }

An easier way to enable/disable intents. Can be used in place of numbers when creating intents.

| name                        | description                           | type                    | access     |
|:----------------------------|:--------------------------------------|:------------------------|:-----------|
| ALL                         | All intents                           | Number                  | **static** |
| NOT_PRIVILEGED              | All intents that don't require whitelisting | Number            | **static** |
| GUILDS                      | Guild events                          | Number                  | **static** |
| GUILD_MEMBERS               | Guild member events (whitelisted)     | Number                  | **static** |
| GUILD_BANS                  | Guild ban events                      | Number                  | **static** |
| GUILD_EMOJIS_AND_STICKERS   | Guild emoji and sticker events        | Number                  | **static** |
| GUILD_INTEGRATIONS          | Guild integration events              | Number                  | **static** |
| GUILD_WEBHOOKS              | Guild webhook events                  | Number                  | **static** |
| GUILD_INVITES               | Guild invite events                   | Number                  | **static** |
| GUILD_VOICE_STATES          | Guild voice state events              | Number                  | **static** |
| GUILD_PRESENCES             | Guild presence events (whitelisted)   | Number                  | **static** |
| GUILD_MESSAGES              | Guild message events                  | Number                  | **static** |
| GUILD_MESSAGE_REACTIONS     | Guild message reaction events         | Number                  | **static** |
| GUILD_MESSAGE_TYPING        | Guild typing events                   | Number                  | **static** |
| DIRECT_MESSAGES             | Direct message events                 | Number                  | **static** |
| DIRECT_MESSAGE_REACTIONS    | Direct message reaction events        | Number                  | **static** |
| DIRECT_MESSAGE_TYPING       | Direct message typing events          | Number                  | **static** |
| GUILD_SCHEDULED_EVENTS      | Guild scheduled events                | Number                  | **static** |

```js
// both Intents.FLAGS.GUILDS and (1 << 0) equal 1
Intents.FLAGS.GUILDS == (1 << 0); // true
```

**Type:** Object

# Methods

## add(...flags)
Adds flags to this [Intents](#constructor) instance.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| ...flags                    | The intents to add                    | Number                  |

```js
// add one or more intents from Intents.FLAGS...
intents.add(Intents.FLAGS.GUILDS, Intents.FLAGS.GUILD_MESSAGES);
```

**Returns:** [Intents](#constructor)

## remove(...flags)
Removes flags from this [Intents](#constructor) instance.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| ...flags                    | The intents to remove                 | Number                  |

```js
// enable all but typing events
intents.add(Intents.FLAGS.ALL);
intents.remove(Intents.FLAGS.GUILD_MESSAGE_TYPING, Intents.FLAGS.DIRECT_MESSAGE_TYPING);
```

**Returns:** [Intents](#constructor)

## has(flag)
Check if this [Intents](#constructor) instance has a flag.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| flag                        | The flag to check for                 | Number                  |

```js
// check if an intents list has an intent
if (intents.has(Intents.FLAGS.GUILDS)) {
    console.log('intents has guilds!');
}
```

**Returns:** Boolean

## toString()
Convert this [Intents](#constructor) instance into a string.

**Returns:** String

## fromString(string)
{: .d-inline-block }

STATIC
{: .label .label }

Convert an intents string into an [Intents](#constructor) instance.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| string                      | The string                            | String                  |

**Returns:** [Intents](#constructor)

# Examples
Create a basic client that listens to all intents:
```js
const { Client, Intents } = require('birb');
new Intents(Intents.FLAGS.ALL);
```
Just listen to guild and guild message events:
```js
const { Intents } = require('birb');
new Intents(Intents.FLAGS.GUILDS, Intents.FLAGS.GUILD_MESSAGES);
```
Only listen to messages in DMs:
```js
const { Intents } = require('birb');
new Intents(Intents.FLAGS.DIRECT_MESSAGES);
```
