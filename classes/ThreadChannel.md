---
layout: default
title: ThreadChannel
parent: Classes
has_children: false
has_toc: true
---

# ThreadChannel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new ThreadChannel(client, data, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |
| options | Object |  | true |  |

# Properties
## client
**Type:** [Client](/classes/Client)

## guild
**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## messages
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** [MessageBlock](/classes/MessageBlock)

## name
**Type:** string

## permissions
**Type:** [ChannelPermissionsBlock](/classes/ChannelPermissionsBlock)

# Methods
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** undefined

## modify(data, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[ThreadChannel](/classes/ThreadChannel)>

## send(message)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## set()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the ThreadChannel's data to the cache.

**Returns:** [ThreadChannel](/classes/ThreadChannel)

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | Object |  | false |  |

**Returns:** Promise<void>

