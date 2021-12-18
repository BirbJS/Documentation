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
The client is the entrypoint to Birb.JS. If you'd
like to learn how to use Birb.JS, head over to our
[docs](https://birb.js.org) or have a quick look at
our [examples](https://birb.js.org/start).
# Constructor
```js
new Client(options)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object | The client options. | false | *none* |

# Properties
## api
{: .d-inline-block }

READONLY
{: .label .label-purple }

Direct access to the client's rest API endpoints.

**Type:** Object

## channels
The client's channel cache.

**Type:** [ChannelBlock](/classes/ChannelBlock)

## devtools
The devtools instance for this client. Only set if
the `@birbjs/devtools` package is installed.

**Type:** any

## guilds
The client's guild cache.

**Type:** [GuildBlock](/classes/GuildBlock)

## me
The client's Discord user.

**Type:** Object or [ClientUser](/classes/ClientUser)

## options
The client's options.

**Type:** Object

## shard
The client's Shard if sharding is enabled. See the
[docs](https://birb.js.org/addons/sharding) for more
information.

**Type:** any

## token
The token of the client.

**Type:** string

## users
The client's user cache.

**Type:** [UserBlock](/classes/UserBlock)

## ws
The client's websocket.

**Type:** [Websocket](/classes/Websocket)

# Methods
## add(fn)
Initilize a new addon to the client.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | Function | The addon's main function. | false | *none* |

**Returns:** [Client](/classes/Client)

## connect(token)
Connect to the Discord gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| token | string | Your bot's token. | false | *none* |

**Returns:** void

## debug(message)
Emit a log in debug mode.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The log message. | false | *none* |

**Returns:** void

## emit(event, args)
Emit an event.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | string | The event name. | false | *none* |
| args | Object |   | false | *none* |

**Returns:** any

## invalidate()
Invalidate the client, forcing the user to restart
the process to use it. Once called, this cannot be
undone (mostly because it would defeat the entire
purpose of this function).

**Returns:** void

## listen(event, callback)
Add an event listener.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | string | The event name. | false | *none* |
| callback | Function |   | false | *none* |

**Returns:** void

## unbind(event)
Undind an event listener.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| event | string | The event name to unbind. | false | *none* |

**Returns:** void

## warn(message)
Emit a warning in debug mode.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | Object | The warning message. | false | *none* |

**Returns:** void

