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
A GuildMember represents a member of a Discord
guild (or "server").
# Constructor
```js
new GuildMember(client, data, guild)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client that this member belongs to. | false | *none* |
| data | any | The data of this member. | false | *none* |
| guild | [Guild](/classes/Guild) | The guild this member is in.  | false | *none* |

# Properties
## avatar
The avatar hash for this member.
**Note:** This is not the same as an avatar URL. Use
the `displayAvatarURL` method to get the avatar URL
of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## client
The client that this member belongs to.

**Type:** [Client](/classes/Client)

## deafened
Whether or not this member is deafened in this
guild's voice channels. If `true`, the member won't
be able to hear anything said in voice channels.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## full
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Whether or not this member has been fully resolved.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## guild
The guild this member is in.

**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The user ID of this member.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## joinedAt
The date this member joined the guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| Date

## muted
Whether or not this member is muted in this guild's
voice channels. If `true`, the member won't be able
to say anything in voice channels.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## nick
The nickname of this member.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## originalUser
{: .d-inline-block }

PROTECTED
{: .label .label-red }

The original user object of this member.

**Type:** any

## pendingMembershipScreening
Whether or not this member is pending membership
screening in this guild. Until membership screening
is passed, the member may not interact with the
guild in any way.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## roles
The roles this member has.

**Type:** [GuildMemberRoleBlock](/classes/GuildMemberRoleBlock)

## timedOutUntil
The date until this member leaves timeout mode. This
will be `null` if the member is not in timeout mode.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| Date

## user
The user related to this member.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| [BaseUser](/classes/BaseUser)

# Methods
## _waitForFull()
Forces the client to wait until the member has been
fully resolved. If the member is in the cache, the
promise will resolve immediately. However, if the
client will fetch the member from the Discord API.

**Returns:** Promise<[GuildMember](/classes/GuildMember)>

## ban(daysToPrune, reason?)
Ban the GuildMember.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| daysToPrune | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## isInTimeout()
Check if this GuildMember is in timeout.

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## kick(reason?)
Kick the GuildMember.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## modify(data, reason?)
Modify the GuildMember.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object | The data to send to the Discord API. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setDeafen(deafen, reason?)
Set this GuildMember's deafened status.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| deafen | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* | The new deafened status. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setMute(mute, reason?)
Set this GuildMember's muted status.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| mute | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* |   | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

## setNick(nickname, reason?)
Set this GuildMember's nickname.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| nickname | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new nickname. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<void>

