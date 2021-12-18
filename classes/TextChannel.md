---
layout: default
title: TextChannel
parent: Classes
has_children: false
has_toc: true
---

# TextChannel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A TextChannel represents any guild text channel on
Discord.
# Constructor
```js
new TextChannel(client, data, options?, guild?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this channel belongs to. | false | *none* |
| data | any | The data of this channel. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |
| guild | [Guild](/classes/Guild) |   | true | *none* |

# Properties
## client
The client this channel belongs to.

**Type:** [Client](/classes/Client)

## guild
The guild this channel belongs to.

**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this channel.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## messages
The messages in this channel.

**Type:** [MessageBlock](/classes/MessageBlock)

## name
The name of this channel.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## permissions
The permission overwrites associated with this
channel.

**Type:** [ChannelPermissionsBlock](/classes/ChannelPermissionsBlock)

# Methods
## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Initialize the data of this channel.

**Returns:** any

## modify(data, reason?)
Send a raw modify request to the Discord API.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to send. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## send(message)
Sends a message to this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |   | false | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## set()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the TextChannel's data to the cache.

**Returns:** [TextChannel](/classes/TextChannel)

## setAutoArchive(minutes, reason?)
Set the auto-archive timeout of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| minutes | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The auto-archive timeout of this channel in minutes. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setNSFW(nsfw, reason?)
Set whether or not this channel is Not Safe For
Wumpus (explict).

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| nsfw | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* | Whether or not this channel is explicit. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setName(name, reason?)
Set the name of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of this channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the overwrites of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** Promise<void>

## setPosition(position, reason?)
Set the position of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| position | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The position of this channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setSlowmode(seconds, reason?)
Sets the slowmode of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| seconds | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The number of seconds of slowmode. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setTopic(topic, reason?)
Set the topic of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| topic | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The topic of this channel. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

