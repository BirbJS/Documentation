---
layout: default
title: GuildChannel
parent: Classes
has_children: false
has_toc: true
---

# GuildChannel
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A GuildChannel represents any channel on Discord
that is associated with a guild.
# Constructor
```js
new GuildChannel(client, data, guild?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this channel belongs to. | false | *none* |
| data | any | The data of this channel. | false | *none* |
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
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

Send a raw API request to modify this channel

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to send. | false | *none* |
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** Promise<[GuildChannel](/classes/GuildChannel)>

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the overwrites of this channel.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** Promise<void>

