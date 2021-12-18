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

**Type:** Object

## author
The author of this message.

**Type:** Object or [BaseUser](/classes/BaseUser)

## channel
The channel this message was sent in.

**Type:** [TextBasedChannel](/classes/TextBasedChannel)

## client
The client this message belongs to.

**Type:** [Client](/classes/Client)

## content
The text content of the message.

**Type:** Object or string

## flags
This message's bitfield flags.

**Type:** number

## guild
The guild this message was sent in, if any.

**Type:** Object or [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of the message.

**Type:** string

## member
The member that sent this message if this message
was sent in a guild.

**Type:** Object or [GuildMember](/classes/GuildMember)

## system
Whether or not this is a system message (e.g. a
welcome message).

**Type:** boolean

## type
The type of message.

**Type:** Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object or Object

## webhookId
The webhook ID if this message was sent by a Discord
webhook.

**Type:** Object or string

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
| reason | string |   | true | *none* |

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
| name | string | The name of the thread. | false | *none* |
| options | Object |   | false | {} |

**Returns:** Promise<void>

## supressEmbeds()
Supress the embeds of this message.

**Returns:** Promise<[Message](/classes/Message)>

## unpin(reason?)
Unpin this message from the channel it was sent in.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | string |   | true | *none* |

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
| edit | boolean |   | false | false |

**Returns:** any

