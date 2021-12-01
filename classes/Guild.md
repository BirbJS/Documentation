---
layout: default
title: Guild
parent: Classes
has_toc: true
---

# Guild
A Guild represents a Discord server.

### Contents
{: .no_toc .text-delta }

- TOC
{:toc}

# Constructor
`new Guild(client, data)`

| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| client                 | The client            | [Client](/classes/Client)        | false    | none        |
| data                   | Raw data from the API | Object                           | false    | none        |

# Properties

## client
The client related to this Guild.

**Type:** [Client](/classes/Client)

## id
The Guild's ID.

**Type:** String

## name
The Guild's name.

**Type:** String

## icon
The Guild's icon hash.

**Type:** String?

## nsfw
Whether or not this Guild has been marked as NSFW.

**Type:** boolean?

## discoverySplash
This guild's discovery splash hash.

**Type:** String?

## banner
This guild's banner hash.

**Type:** String?

## description
This guild's description.

**Type:** String?

## verificationLevel
This guild's [verification level](https://discord.com/developers/docs/resources/guild#guild-object-verification-level).

**Type:** [VerificationLevel](/enums/VerificationLevel)

## defaultNotifications
This guild's [default message notification level](https://discord.com/developers/docs/resources/guild#guild-object-default-message-notification-level).

**Type:** [NotificationLevel](/enums/NotificationLevel)

## available
Whether or not this Guild is available to this client.

**Type:** boolean

## systemChannelId
The ID of the system notifications channel.

**Type:** String?

## ownerId
The ID of the Guild owner.

**Type:** String

## large
Whether or not this Guild is considered large.

**Type:** String?

## afkChannelId
The ID of the AFK voice channel.

**Type:** String?

## explicitContentFilter
The explicit content filter level for this Guild.

**Type:** [ExplicitContentFilterLevel](/enums/ExplicitContentFilterLevel)

## maxMembers
The maximum amount of members this Guild can have.

**Type:** number?

## preferredLocale
This Guild's preferred locale.

**Type:** String?

## mfaLevel
The level of MFA required for this Guild's staff members.

**Type:** [MFALevel](/enums/MFALevel)

## vanityCode
This Guild's vanity invite code, if it has one.

**Type:** String?

## nsfwLevel
The Discord-defined NSFW level related to this Guild's content.

**Type:** [NSFWLevel](/enums/NSFWLevel)

## maxVideoChannelUsers
The maximum amount of users allowed in a video channel.

**Type:** number?

## boosterCount
The amount of users who have Nitro boosted for this Guild.

**Type:** number?

## splash
This Guild's splash hash.

**Type:** String?

## memberCount
This Guild's member count.

**Type:** number?

## boostTier
This Guild's Nitro booster tier.

**Type:** number

## rulesChannelId
This ID of this Guild's rules channel, if it has one.

**Type:** String?

## afkTimeout
The amount of time, in seconds, it takes for an inactive user to be moved to the AFK voice channel.

**Type:** number

## roles
This Guild's roles block.

**Type:** [RoleBlock](/classes/RolesBlock)

# Methods

## listen(event, listener)
{: .d-inline-block }

EVENT LISTENER
{: .label .label-purple }

Registers a listener for the specified event.

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| event                       | The event to listen to                | String                  | false          |
| listener                    | The function to be ran when emitted   | Function                | false          |

```js
client.listen('message', message => {
    if (message.content === 'hi') {
        message.reply('hello!');
    }
});
```

**Returns:** void

# Examples
Send `hello!` when a member says `hi`:
```js
const { Client, Intents } = require('birb');
const client = new Client({
    intents: new Intents(Intents.FLAGS.ALL)
});

client.listen('message', (message) => {
    if (message.content === 'hi') {
        message.reply('hello!');
    }
});

client.connect("token")
```
