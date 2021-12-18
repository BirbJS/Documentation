---
layout: default
title: TextBasedChannel
parent: Classes
has_children: false
has_toc: true
---

# TextBasedChannel
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A TextBasedChannel represents any guild channel that
allows messages to be sent and received.
# Constructor
```js
new TextBasedChannel(client, data, options?, guild?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this channel belongs to. | false | *none* |
| data | any | The data of this channel. | false | *none* |
| options | Object |   | true | *none* |
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

**Type:** string

## messages
The messages in this channel.

**Type:** [MessageBlock](/classes/MessageBlock)

## name
The name of this channel.

**Type:** string

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
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

Send a raw API request to modify this channel

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to send. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[GuildChannel](/classes/GuildChannel)>

## send(message)
Sends a message to this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |   | false | *none* |

**Returns:** Promise<[Message](/classes/Message)>

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the overwrites of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | Object |   | false | *none* |

**Returns:** Promise<void>

