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
# Constructor
```js
new TextBasedChannel(client, data, options?, guild?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| data | any |  | false |  |
| options | Object |  | true |  |
| guild | [Guild](classes/Guild) |  | true |  |

# Properties
## client
**Type:** [Client](classes/Client)

## guild
**Type:** [Guild](classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## messages
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** [MessageBlock](classes/MessageBlock)

## name
**Type:** string

## permissions
**Type:** [ChannelPermissionsBlock](classes/ChannelPermissionsBlock)

# Methods
## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** undefined | Object

## modify(data, reason?)
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[GuildChannel](classes/GuildChannel)>

## send(message)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |  | false |  |

**Returns:** Promise<[Message](classes/Message)>

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | Object |  | false |  |

**Returns:** Promise<void>

