---
layout: default
title: Intents
parent: Classes
---

# Intents
The Discord API uses intents to determine what events should be sent to connected clients. Intents are now **required** when connecting. You may use `Intents.FLAGS.ALL` to enable all intents, and `Intents.FLAGS.NOT_PRIVILEGED` to enable all intents that don't require approval (for verified bots).

## Constructor
`new Intents(...flags)`

| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| ...flags               | The intents to use    | Number (or from Intents.FLAGS)   | false    | none        |

# Properties

| name                        | description                           | type                    | access     |
|:----------------------------|:--------------------------------------|:------------------------|:-----------|
| FLAGS                       | A list of intents that can be used    | Object                  | **static** |
| FLAGS.ALL                   | All intents                           | Number                  | **static** |
| FLAGS.NOT_PRIVILEGED        | All intents that don't require whitelisting | Number            | **static** |
| FLAGS.GUILDS                | Guild events                          | Number                  | **static** |
| FLAGS.GUILD_MEMBERS         | Guild member events (whitelisted)     | Number                  | **static** |
| FLAGS.GUILD_BANS            | Guild ban events                      | Number                  | **static** |
| FLAGS.GUILD_EMOJIS_AND_STICKERS | Guild emoji and sticker events    | Number                  | **static** |
| FLAGS.GUILD_INTEGRATIONS    | Guild integration events              | Number                  | **static** |
| FLAGS.GUILD_WEBHOOKS        | Guild webhook events                  | Number                  | **static** |
| FLAGS.GUILD_INVITES         | Guild invite events                   | Number                  | **static** |
| FLAGS.GUILD_VOICE_STATES    | Guild voice state events              | Number                  | **static** |
| FLAGS.GUILD_PRESENCES       | Guild presence events (whitelisted)   | Number                  | **static** |
| FLAGS.GUILD_MESSAGES        | Guild message events                  | Number                  | **static** |
| FLAGS.GUILD_MESSAGE_REACTIONS | Guild message reaction events       | Number                  | **static** |
| FLAGS.GUILD_MESSAGE_TYPING  | Guild typing events                   | Number                  | **static** |
| FLAGS.DIRECT_MESSAGES       | Direct message events                 | Number                  | **static** |
| FLAGS.DIRECT_MESSAGE_REACTIONS | Direct message reaction events     | Number                  | **static** |
| FLAGS.DIRECT_MESSAGE_TYPING | Direct message typing events          | Number                  | **static** |
| FLAGS.GUILD_SCHEDULED_EVENTS | Guild scheduled events               | Number                  | **static** |

## Examples
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
