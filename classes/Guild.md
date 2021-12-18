---
layout: default
title: Guild
parent: Classes
has_children: false
has_toc: true
---

# Guild
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A Guild represents a Discord server.
# Constructor
```js
new Guild(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client that this guild belongs to. | false | *none* |
| data | any | The data for this guild.  | false | *none* |

# Properties
## afkChannelId
The ID of the guild's AFK channel.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## afkTimeout
The amount of seconds to wait before moving AFK
members to the AFK voice channel.

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## approximateMemberCount
The approximate amount of members in this guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## approximatePresenceCount
The approximate amount of online members in this
guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## available
Whether or not this guild is available to this
client. **You should check this is set to `true`
before performing actions on guilds.**

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## banner
The guild's banner hash.
**Note:** This is not the same as an banner URL.
Use the `getBannerURL` method to get the icon URL of
this guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## boostTier
The boost tier of this guild.

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## boosterCount
The amount of members who have used Discord Nitro
to boost this guild (or have purchased a Nitro boost
on its own for this guild).

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## channels
The channels this guild has.

**Type:** default

## client
The client this Guild belongs to.

**Type:** [Client](/classes/Client)

## defaultNotifications
The default notification level of this guild.

**Type:** [NotificationLevel](/enums/NotificationLevel)

## description
The guild's description.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## discoverySplash
The guild's discovery splash hash.
**Note:** This is not the same as a splash URL. Use
the `getSplashURL` method to get the splash URL of
this guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## explicitContentFilter
The setting of the explicit content filter for this
guild.

**Type:** [ExplicitContentFilterLevel](/enums/ExplicitContentFilterLevel)

## icon
The guild's icon hash.
**Note:** This is not the same as an icon URL. Use
the `getIconURL` method to get the icon URL of this
guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this Guild.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## large
Whether or not this guild is deemed 'large' (at
which point Discord will not automatically send a
list of members).

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## maxMembers
The maximum amount of members allowed in this guild.
Reach out to [Discord support](https://dis.gd/support)
if you're getting close to this limit and need it
increased.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## maxVideoChannelUsers
The maximum amount of video channel members.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## memberCount
The member count of this guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## members
The members this guild has.

**Type:** [GuildMemberBlock](/classes/GuildMemberBlock)

## mfaLevel
The multi-factor authentication requirement level
for this guild's staff members.

**Type:** [MFALevel](/enums/MFALevel)

## name
The name of this Guild.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## nsfw
Whether or not Discord has marked this guild as Not
Safe For Wumpus (explicit).

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## nsfwLevel
The Not Safe For Wumpus (explicit) level Discord has
assigned to this guild. Discord uses this to block
NSFW servers on iOS.

**Type:** [NSFWLevel](/enums/NSFWLevel)

## ownerId
The ID of the owner of this guild.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## preferredLocale
The preferred locale (language) for this Guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## roles
The roles this guild has.

**Type:** [RoleBlock](/classes/RoleBlock)

## rulesChannelId
The channel ID of the guild's rules or guidelines
channel.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## splash
The splash hash of this guild.
**Note:** This is not the same as a splash URL.
Use the `getSplashURL` method to get the splash URL
of this guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## systemChannelId
The ID of this guild's system channel where join
notifications, boost messages, etc. are sent.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## vanityCode
The vanity invite code this guild owns. `null` if it
doesn't have one.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## verificationLevel
The verification level of this guild.

**Type:** [VerificationLevel](/enums/VerificationLevel)

# Methods
## leave()
Leave the Guild.

**Returns:** Promise<void>

## modify(data, reason?)
Modify the Guild.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object | The data to send to the Discord API. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setAfkChannel(channel, reason?)
Set this Guild's AFK timeout channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The AFK timeout channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setAfkTimeout(seconds, reason?)
Change this Guild's AFK timeout.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| seconds | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The AFK timeout in seconds. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setBoostProgressBar(toggle, reason?)
Toggle the Guild's booster progress bar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| toggle | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | Whether or not to show the booster progress bar. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setDefaultNotifications(level, reason?)
Change this Guild's default notifications level.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| level | [NotificationLevel](/enums/NotificationLevel) | The new notification level for the Guild. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setDescription(description, reason?)
Set the Guild's description.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| description | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new description. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setExplicitContentFilter(level, reason?)
Change this Guild's explicit content filter level.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| level | [ExplicitContentFilterLevel](/enums/ExplicitContentFilterLevel) | The new explicit content filter level for the Guild. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setName(name, reason?)
Change this Guild's name.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new name for the Guild. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setPreferredLocale(locale, reason?)
Set the Guild's preferred locale.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| locale | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new locale. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setPublicUpdatesChannel(channel, reason?)
Set this Guild's public updates channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setRulesChannel(channel, reason?)
Set this Guild's rules channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setSystemChannel(channel, reason?)
Set this Guild's system messages channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setVerificationLevel(level, reason?)
Change this Guild's verification level.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| level | [VerificationLevel](/enums/VerificationLevel) | The new verification level for the Guild. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## toString()
Convert this Guild into a a string (the name).

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

