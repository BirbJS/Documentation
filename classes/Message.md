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
| data | any | The data of the message.
 | false | *none* |

# Properties
## attachments
Any attachments that were sent with this message.

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## author
The author of this message.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or [BaseUser](/classes/BaseUser)

## channel
The channel this message was sent in.

**Type:** [TextBasedChannel](/classes/TextBasedChannel)

## client
The client this message belongs to.

**Type:** [Client](/classes/Client)

## content
The text content of the message.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## flags
This message's bitfield flags.

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## guild
The guild this message was sent in, if any.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of the message.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## member
The member that sent this message if this message
was sent in a guild.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or [GuildMember](/classes/GuildMember)

## system
Whether or not this is a system message (e.g. a
welcome message).

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## type
The type of message.

**Type:** DEFAULT or RECIPIENT_ADD or RECIPIENT_REMOVE or CALL or CHANNEL_NAME_CHANGE or CHANNEL_ICON_CHANGE or CHANNEL_PINNED_MESSAGE or GUILD_MEMBER_JOIN or USER_PREMIUM_GUILD_SUBSCRIPTION or USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_1 or USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_2 or USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_3 or CHANNEL_FOLLOW_ADD or GUILD_DISCOVERY_DISQUALIFIED or GUILD_DISCOVERY_REQUALIFIED or GUILD_DISCOVERY_GRACE_PERIOD_INITIAL_WARNING or GUILD_DISCOVERY_GRACE_PERIOD_FINAL_WARNING or THREAD_CREATED or REPLY or CHAT_INPUT_COMMAND or THREAD_STARTER_MESSAGE or GUILD_INVITE_REMINDER or CONTEXT_MENU_COMMAND

## webhookId
The webhook ID if this message was sent by a Discord
webhook.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

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

