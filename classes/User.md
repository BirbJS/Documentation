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
# Constructor
```js
new User(client, data)
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

## dmChannel
**Type:** any

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
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## fetch(options?)
Fetch this user again.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | true |  |

**Returns:** Promise<[User](/classes/User)>

## getAvatar(options?)
Generate a link to the user's avatar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | true |  |

**Returns:** string

## getBanner(options?)
Generate a link to the user's avatar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | true |  |

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
| content | string |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## set()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Set the User's data to the cache.

**Returns:** [User](/classes/User)

## toString()
Convert this User into a mention (string).

**Returns:** string

## retrieveOrBuildPartial(client, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Either fetch a User from the cache or return a
PartialUser instance to avoid fetching from the API.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client to use. | false |  |
| data | any | The data on the user (`id` is required). | false |  |

**Returns:** [User](/classes/User) | [PartialUser](/classes/PartialUser)

## toIdOnly(user)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable |  | false |  |

**Returns:** string

