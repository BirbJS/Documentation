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
# Constructor
```js
new Guild(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |

# Properties
## afkChannelId
<<<<<<< Updated upstream
**Type:** Object | string
=======
The ID of the guild's AFK channel.

**Type:** Object or string
>>>>>>> Stashed changes

## afkTimeout
**Type:** number

## approximateMemberCount
<<<<<<< Updated upstream
**Type:** Object | number

## approximatePresenceCount
**Type:** Object | number
=======
The approximate amount of members in this guild.

**Type:** Object or number

## approximatePresenceCount
The approximate amount of online members in this
guild.

**Type:** Object or number
>>>>>>> Stashed changes

## available
**Type:** boolean

## banner
<<<<<<< Updated upstream
**Type:** Object | string
=======
The guild's banner hash.
**Note:** This is not the same as an banner URL.
Use the `getBannerURL` method to get the icon URL of
this guild.

**Type:** Object or string
>>>>>>> Stashed changes

## boostTier
**Type:** number

## boosterCount
<<<<<<< Updated upstream
**Type:** Object | number
=======
The amount of members who have used Discord Nitro
to boost this guild (or have purchased a Nitro boost
on its own for this guild).

**Type:** Object or number
>>>>>>> Stashed changes

## channels
**Type:** default

## client
**Type:** [Client](/classes/Client)

## defaultNotifications
**Type:** [NotificationLevel](/enums/NotificationLevel)

## description
<<<<<<< Updated upstream
**Type:** Object | string

## discoverySplash
**Type:** Object | string
=======
The guild's description.

**Type:** Object or string

## discoverySplash
The guild's discovery splash hash.
**Note:** This is not the same as a splash URL. Use
the `getSplashURL` method to get the splash URL of
this guild.

**Type:** Object or string
>>>>>>> Stashed changes

## explicitContentFilter
**Type:** [ExplicitContentFilterLevel](/enums/ExplicitContentFilterLevel)

## icon
<<<<<<< Updated upstream
**Type:** Object | string
=======
The guild's icon hash.
**Note:** This is not the same as an icon URL. Use
the `getIconURL` method to get the icon URL of this
guild.

**Type:** Object or string
>>>>>>> Stashed changes

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## large
**Type:** boolean

## maxMembers
<<<<<<< Updated upstream
**Type:** Object | number

## maxVideoChannelUsers
**Type:** Object | number

## memberCount
**Type:** Object | number
=======
The maximum amount of members allowed in this guild.
Reach out to [Discord support](https://dis.gd/support)
if you're getting close to this limit and need it
increased.

**Type:** Object or number

## maxVideoChannelUsers
The maximum amount of video channel members.

**Type:** Object or number

## memberCount
The member count of this guild.

**Type:** Object or number
>>>>>>> Stashed changes

## members
**Type:** [GuildMemberBlock](/classes/GuildMemberBlock)

## mfaLevel
**Type:** [MFALevel](/enums/MFALevel)

## name
**Type:** string

## nsfw
**Type:** boolean

## nsfwLevel
**Type:** [NSFWLevel](/enums/NSFWLevel)

## ownerId
**Type:** string

## preferredLocale
<<<<<<< Updated upstream
**Type:** Object | string
=======
The preferred locale (language) for this Guild.

**Type:** Object or string
>>>>>>> Stashed changes

## roles
**Type:** [RoleBlock](/classes/RoleBlock)

## rulesChannelId
<<<<<<< Updated upstream
**Type:** Object | string

## splash
**Type:** Object | string

## systemChannelId
**Type:** Object | string

## vanityCode
**Type:** Object | string
=======
The channel ID of the guild's rules or guidelines
channel.

**Type:** Object or string

## splash
The splash hash of this guild.
**Note:** This is not the same as a splash URL.
Use the `getSplashURL` method to get the splash URL
of this guild.

**Type:** Object or string

## systemChannelId
The ID of this guild's system channel where join
notifications, boost messages, etc. are sent.

**Type:** Object or string

## vanityCode
The vanity invite code this guild owns. `null` if it
doesn't have one.

**Type:** Object or string
>>>>>>> Stashed changes

## verificationLevel
**Type:** [VerificationLevel](/enums/VerificationLevel)

# Methods
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## leave()
Leave the Guild.

**Returns:** Promise<void>

## modify(data, reason?)
Modify the Guild.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object | The data to send to the Discord API. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## set()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Set the Guild's data to the cache.

**Returns:** [Guild](/classes/Guild)

## setAfkChannel(channel, reason?)
Set this Guild's AFK timeout channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The AFK timeout channel. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setAfkTimeout(seconds, reason?)
Change this Guild's AFK timeout.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| seconds | number | The AFK timeout in seconds. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setBoostProgressBar(toggle, reason?)
Toggle the Guild's booster progress bar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| toggle | number | Whether or not to show the booster progress bar. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setDefaultNotifications(level, reason?)
Change this Guild's default notifications level.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| level | [NotificationLevel](/enums/NotificationLevel) | The new notification level for the Guild. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setDescription(description, reason?)
Set the Guild's description.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| description | string | The new description. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setExplicitContentFilter(level, reason?)
Change this Guild's explicit content filter level.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| level | [ExplicitContentFilterLevel](/enums/ExplicitContentFilterLevel) | The new explicit content filter level for the Guild. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setName(name, reason?)
Change this Guild's name.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The new name for the Guild. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setPreferredLocale(locale, reason?)
Set the Guild's preferred locale.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| locale | string | The new locale. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setPublicUpdatesChannel(channel, reason?)
Set this Guild's public updates channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The channel. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setRulesChannel(channel, reason?)
Set this Guild's rules channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The channel. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setSystemChannel(channel, reason?)
Set this Guild's system messages channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| channel | ChannelResolvable | The channel. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setVerificationLevel(level, reason?)
Change this Guild's verification level.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| level | [VerificationLevel](/enums/VerificationLevel) | The new verification level for the Guild. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## toString()
Convert this Guild into a a string (the name).

**Returns:** string

