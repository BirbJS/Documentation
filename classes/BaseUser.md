---
layout: default
title: BaseUser
parent: Classes
has_children: false
has_toc: true
---

# BaseUser
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A BaseUser is a model user that is not a partial
user. It is extended upon by the `User` and
`ClientUser` classes.
# Constructor
```js
new BaseUser(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client that this user belongs to. | false | *none* |
| data | any | The data to use to build this user.
 | false | *none* |

# Properties
## accentColor
The accent color of this user represented as a hex
color code (string).

**Type:** Object | string

## avatar
The avatar hash of this user.
**Note:** This is not the same as an avatar URL. Use
the `displayAvatarURL` method to get the avatar URL
of this user.

**Type:** Object | string

## banner
The banner hash of this user.
**Note:** This is not the same as an banner URL. Use
the `getBanner` method to get the banner URL of this
user.

**Type:** Object | string

## bot
Whether or not this user is a bot.

**Type:** boolean

## client
The client that this user belongs to.

**Type:** [Client](/classes/Client)

## discriminator
The discriminator of this user.

**Type:** string

## flags
The flags of this user as a bitfield (string).

**Type:** Object | string

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this user.

**Type:** string

## system
Whether or not this user is a part of the official
Discord Urgent Message System.

**Type:** boolean

## tag
The tag of this user.

**Type:** string

## username
The username of this user.

**Type:** string

# Methods
## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

