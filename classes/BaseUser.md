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
# Constructor
```js
new BaseUser(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |

# Properties
<<<<<<< Updated upstream
## accent_color
**Type:** Object | string

## avatar
**Type:** Object | string

## banner
**Type:** Object | string
=======
## accentColor
The accent color of this user represented as a hex
color code (string).

**Type:** Object or string

## avatar
The avatar hash of this user.
**Note:** This is not the same as an avatar URL. Use
the `displayAvatarURL` method to get the avatar URL
of this user.

**Type:** Object or string

## banner
The banner hash of this user.
**Note:** This is not the same as an banner URL. Use
the `getBanner` method to get the banner URL of this
user.

**Type:** Object or string
>>>>>>> Stashed changes

## bot
**Type:** boolean

## client
**Type:** [Client](/classes/Client)

## discriminator
**Type:** string

## flags
<<<<<<< Updated upstream
**Type:** Object | string
=======
The flags of this user as a bitfield (string).

**Type:** Object or string
>>>>>>> Stashed changes

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## system
**Type:** boolean

## tag
**Type:** string

## username
**Type:** string

# Methods
## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

