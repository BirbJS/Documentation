---
layout: default
title: ThreadChannel
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# ThreadChannel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A ThreadChannel represents a thread on Discord.
# Constructor
```js
new ThreadChannel(client, data, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client this channel belongs to. | false | *none* |
| data | any | The data of this channel. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

# Properties
## client
The client this channel belongs to.

**Type:** [Client](/ref/classes/Client)

## guild
The guild this channel belongs to.

**Type:** [Guild](/ref/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this channel.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## messages
The messages in this channel.

**Type:** [MessageBlock](/ref/classes/MessageBlock)

## name
The name of this channel.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## permissions
The permission overwrites associated with this
channel.

**Type:** [ChannelPermissionsBlock](/ref/classes/ChannelPermissionsBlock)

# Methods
## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Initialize the data of this channel.

**Returns:** any

## modify(data, reason?)
Send a modify request to the API.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to send. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[ThreadChannel](/ref/classes/ThreadChannel)>

## send(message)
Sends a message to this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |   | false | *none* |

**Returns:** Promise<[Message](/ref/classes/Message)>

## set()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the ThreadChannel's data to the cache.

**Returns:** [ThreadChannel](/ref/classes/ThreadChannel)

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the overwrites of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** Promise<void>

