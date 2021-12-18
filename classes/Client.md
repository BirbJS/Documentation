---
layout: default
title: Client
parent: Classes
has_children: false
has_toc: true
---

# Client
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Client(options)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | false |  |

# Properties
## api
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** Object

## channels
**Type:** [ChannelBlock](/classes/ChannelBlock)

## devtools
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Type:** any

## events
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Type:** any

## guilds
**Type:** [GuildBlock](/classes/GuildBlock)

## me
<<<<<<< Updated upstream
**Type:** Object | [ClientUser](/classes/ClientUser)
=======
The client's Discord user.

**Type:** Object or [ClientUser](/classes/ClientUser)
>>>>>>> Stashed changes

## options
**Type:** Object

## shard
**Type:** any

## token
**Type:** string

## users
**Type:** [UserBlock](/classes/UserBlock)

## valid
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Type:** boolean

## ws
**Type:** [Websocket](/classes/Websocket)

# Methods
## add(fn)
Initilize a new addon to the client.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | Function | The addon's main function. | false |  |

**Returns:** [Client](/classes/Client)

## connect(token)
Connect to the Discord gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| token | string | Your bot's token. | false |  |

**Returns:** void

## debug(message)
Emit a log in debug mode.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The log message. | false |  |

**Returns:** void

## emit(event, args)
Emit an event.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | string | The event name. | false |  |
| args | Object |  | false |  |

**Returns:** any

## invalidate()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Invalidate the client, forcing the user to restart
the process to use it. Once called, this cannot be
undone (mostly because it would defeat the entire
purpose of this function).

**Returns:** void

## listen(event, callback)
Add an event listener.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | string | The event name. | false |  |
| callback | Function |  | false |  |

**Returns:** void

## listenIfNotRegistered(event, callback)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Only registers the provided event if it isn't
already registered.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | EventResolvable |  | false |  |
| callback | Function |  | false |  |

**Returns:** void

## logHttp(message)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Log a HTTP event.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The event data. | false |  |

**Returns:** void

## logReceive(message)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Log a packet received from the gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The packet data. | false |  |

**Returns:** void

## logSend(message)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Log a packet sent to the gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The packet data. | false |  |

**Returns:** void

## unbind(event)
Undind an event listener.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | string | The event name to unbind. | false |  |

**Returns:** void

## warn(message)
Emit a warning in debug mode.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The warning message. | false |  |

**Returns:** void

