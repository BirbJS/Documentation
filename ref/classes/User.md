---
layout: default
title: User
parent: Classes
grand_parent: Reference
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
| client | [Client](/ref/classes/Client) | The client that instantiated this User. | false | *none* |
| data | any | The data for this User.  | false | *none* |

# Properties
## accentColor
The accent color of this user represented as a hex color code string.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## avatar
The avatar hash of this user.
**Note**: This is not the same as an avatar URL.
Use `BaseUser#displayAvatarURL()` method to get the avatar URL of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## banner
The banner hash of this user.
**Note:** This is not the same as an banner URL.
Use `BaseUser#getBanner()` method to get the banner URL of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## bot
Whether or not this user is a bot.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## client
The client this user belongs to.

**Type:** [Client](/ref/classes/Client)

## discriminator
The discriminator of this user.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## dmChannel
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Raw data on this user's DM channel.

**Type:** any

## flags
The flags of this user.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

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
## fetch(options?)
Fetch this user again.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** Promise<[User](/ref/classes/User)>

## getAvatar(options?)
Generate a link to the user's avatar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## getBanner(options?)
Generate a link to the user's avatar.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## hasDefaultAvatar()
Determine if the user's avatar is default.

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## send(content)
Send a message to the user.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| content | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

**Returns:** Promise<[Message](/ref/classes/Message)>

## toString()
Convert this User into a mention (string).

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

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

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

