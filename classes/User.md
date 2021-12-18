---
layout: default
title: User
parent: Classes
has_children: false
has_toc: true
---

# User
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A User represents any Discord user.
# Constructor
```js
new User(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client that instantiated this User. | false | *none* |
| data | any | The data for this User.
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

## dmChannel
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Raw data on this user's DM channel.

**Type:** any

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
## fetch(options?)
Fetch this user again.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |   | true | *none* |

**Returns:** Promise<[User](/classes/User)>

## getAvatar(options?)
Generate a link to the user's avatar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |   | true | *none* |

**Returns:** string

## getBanner(options?)
Generate a link to the user's avatar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |   | true | *none* |

**Returns:** string

## hasDefaultAvatar()
Determine if the user's avatar is default.

**Returns:** boolean

## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

## send(content)
Send a message to the user.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| content | string |   | false | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## toString()
Convert this User into a mention (string).

**Returns:** string

## toIdOnly(user)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Converts a UserResolvable to a user ID (string).

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable | The user to convert. | false | *none* |

**Returns:** string

