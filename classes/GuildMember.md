---
layout: default
title: GuildMember
parent: Classes
has_children: false
has_toc: true
---

# GuildMember
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildMember(client, data, guild)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |
| guild | [Guild](/classes/Guild) |  | false |  |

# Properties
## avatar
<<<<<<< Updated upstream
**Type:** Object | string
=======
The avatar hash for this member.
**Note:** This is not the same as an avatar URL. Use
the `displayAvatarURL` method to get the avatar URL
of this user.

**Type:** Object or string
>>>>>>> Stashed changes

## client
**Type:** [Client](/classes/Client)

## deafened
**Type:** boolean

## full
**Type:** boolean

## guild
**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## joinedAt
<<<<<<< Updated upstream
**Type:** Object | Date
=======
The date this member joined the guild.

**Type:** Object or Date
>>>>>>> Stashed changes

## muted
**Type:** boolean

## nick
<<<<<<< Updated upstream
**Type:** Object | string
=======
The nickname of this member.

**Type:** Object or string
>>>>>>> Stashed changes

## originalUser
**Type:** any

## pendingMembershipScreening
**Type:** boolean

## roles
**Type:** [GuildMemberRoleBlock](/classes/GuildMemberRoleBlock)

## timedOutUntil
<<<<<<< Updated upstream
**Type:** Object | Date

## user
**Type:** Object | [BaseUser](/classes/BaseUser)
=======
The date until this member leaves timeout mode. This
will be `null` if the member is not in timeout mode.

**Type:** Object or Date

## user
The user related to this member.

**Type:** Object or [BaseUser](/classes/BaseUser)
>>>>>>> Stashed changes

# Methods
## _waitForFull()
**Returns:** Promise<[GuildMember](/classes/GuildMember)>

## ban(daysToPrune, reason?)
Ban the GuildMember.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| daysToPrune | number |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## isInTimeout()
Check if this GuildMember is in timeout.

**Returns:** boolean

## kick(reason?)
Kick the GuildMember.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | string |  | true |  |

**Returns:** Promise<void>

## modify(data, reason?)
Modify the GuildMember.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object | The data to send to the Discord API. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## set()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Returns:** [GuildMember](/classes/GuildMember)

## setDeafen(deafen, reason?)
Set this GuildMember's deafened status.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| deafen | boolean | The new deafened status. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setMute(mute, reason?)
Set this GuildMember's muted status.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| mute | boolean |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

## setNick(nickname, reason?)
Set this GuildMember's nickname.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| nickname | string | The new nickname. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<void>

