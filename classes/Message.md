---
layout: default
title: Message
parent: Classes
has_children: false
has_toc: true
---

# Message
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A Message represents a message in any channel on
Discord.
# Constructor
```js
new Message(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this message belongs to. | false | *none* |
| data | any | The data of the message.  | false | *none* |

# Properties
## attachments
Any attachments that were sent with this message.

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## author
The author of this message.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| [BaseUser](/classes/BaseUser)

## channel
The channel this message was sent in.

**Type:** [TextBasedChannel](/classes/TextBasedChannel)

## client
The client this message belongs to.

**Type:** [Client](/classes/Client)

## content
The text content of the message.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## flags
This message's bitfield flags.

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## guild
The guild this message was sent in, if any.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of the message.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## member
The member that sent this message if this message
was sent in a guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| [GuildMember](/classes/GuildMember)

## system
Whether or not this is a system message (e.g. a
welcome message).

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## type
The type of message.

**Type:** DEFAULT \| RECIPIENT_ADD \| RECIPIENT_REMOVE \| CALL \| CHANNEL_NAME_CHANGE \| CHANNEL_ICON_CHANGE \| CHANNEL_PINNED_MESSAGE \| GUILD_MEMBER_JOIN \| USER_PREMIUM_GUILD_SUBSCRIPTION \| USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_1 \| USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_2 \| USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_3 \| CHANNEL_FOLLOW_ADD \| GUILD_DISCOVERY_DISQUALIFIED \| GUILD_DISCOVERY_REQUALIFIED \| GUILD_DISCOVERY_GRACE_PERIOD_INITIAL_WARNING \| GUILD_DISCOVERY_GRACE_PERIOD_FINAL_WARNING \| THREAD_CREATED \| REPLY \| CHAT_INPUT_COMMAND \| THREAD_STARTER_MESSAGE \| GUILD_INVITE_REMINDER \| CONTEXT_MENU_COMMAND

## webhookId
The webhook ID if this message was sent by a Discord
webhook.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## crosspost()
Crosspost this message to channels that are
following the channel this message was sent in.

**Returns:** Promise<[Message](/classes/Message)>

## delete()
Delete this message.

**Returns:** Promise<void>

## edit(message)
Edit this message. Can only be performed if the
message was sent by this client.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |   | false | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## modify(data)
Send a raw API request to edit this message.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to send. | false | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## pin(reason?)
Pin this message to the channel it was sent in.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## reply(message)
Send an inline reply to this message.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |   | false | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## startThread(name, options)
Start a thread from this message.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the thread. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | {} |

**Returns:** Promise<void>

## supressEmbeds()
Supress the embeds of this message.

**Returns:** Promise<[Message](/classes/Message)>

## unpin(reason?)
Unpin this message from the channel it was sent in.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## buildApiMessage(data, edit)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Build an API message.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | MessageContent |   | false | *none* |
| edit | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* |   | false | false |

**Returns:** any

