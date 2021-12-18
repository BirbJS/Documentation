---
layout: default
title: ClientUser
parent: Classes
has_children: false
has_toc: true
---

# ClientUser
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Represents the user that is logged in to the client.
# Constructor
```js
new ClientUser(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this user belongs to. | false | *none* |
| data | any | The data of this user.
 | false | *none* |

# Properties
## accentColor
The accent color of this user represented as a hex color code string.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## avatar
The avatar hash of this user.
**Note**: This is not the same as an avatar URL.
Use `BaseUser#displayAvatarURL()` method to get the avatar URL of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## banner
The banner hash of this user.
**Note:** This is not the same as an banner URL.
Use `BaseUser#getBanner()` method to get the banner URL of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## bot
Whether or not this user is a bot.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## client
The client this user belongs to.

**Type:** [Client](/classes/Client)

## discriminator
The discriminator of this user.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## flags
The flags of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this user.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## system
Whether or not this user is a system account.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## tag
The tag of this user.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## username
The username of this user.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## setName(name)
Set the username of the user.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

**Returns:** Promise<void>

## updatePresence(options)
Updates the user's presence.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | {} |

**Returns:** void

