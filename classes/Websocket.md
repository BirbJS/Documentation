---
layout: default
title: Websocket
parent: Classes
has_children: false
has_toc: true
---

# Websocket
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Creates a websocket connection to a Discord gateway.
# Constructor
```js
new Websocket(client, domain)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) | The client. | false |  |
| domain | string | The domain to connect to. | false |  |

# Properties
## buffer
**Type:** any

## client
**Type:** [Client](classes/Client)

## doNotReconnect
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** boolean

## domain
**Type:** string

## encoding
**Type:** string

## expectedGuilds
**Type:** Set<string>

## heartbeatInterval
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** Object

## lastHeartbeat
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** number

## lastHeartbeatAcked
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** boolean

## lastResume
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** number

## lastSequenceIdentifier
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** Object

## ping
**Type:** number

## schedulerLoop
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** Timer

## sessionIdentifier
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** Object | string

## status
**Type:** [WebsocketStatus](enums/WebsocketStatus)

## url
**Type:** URL

## ws
**Type:** WebSocket

# Methods
## cleanup()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Clean up the websocket.

**Returns:** void

## close(code?)
Close the websocket.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| code | number |  | true |  |

**Returns:** void

## connect()
Connect to the gateway.

**Returns:** void

## generateURL()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** URL

## heartbeat()
Send a heartbeat to the gateway.

**Returns:** Promise<void>

## identify()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Send an identify packet to the gateway.

**Returns:** void

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** void

## isClosed()
Check if the websocket is closed.

**Returns:** boolean

## isConnected()
Check if the websocket is connected.

**Returns:** boolean

## isConnecting()
Check if the websocket is connecting.

**Returns:** boolean

## onClose(code)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Process the websocket closing.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| code | number | The closing code. | false |  |

**Returns:** Promise<void>

## onOpen()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Process the websocket opening.

**Returns:** void

## onPacket(body)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Process a packet.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| body | any |  | false |  |

**Returns:** Promise<void>

## pack(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** any

## preventReconnect(value?)
Prevent reconnection.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| value | boolean |  | true |  |

**Returns:** void

## processPacket(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** any

## reconnect()
Reconnect to the gateway.

**Returns:** void

## scheduler()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Creates a loop that will manage repeating tasks. It
will call it's method every 50ms.

**Returns:** void

## send(data)
Send a packet to the gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object | The data to send. | false |  |

**Returns:** void

## setSessionIdentifier(sessionIdentifier)
Set the websocket's session identifier.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| sessionIdentifier | string | The session identifier to set. | false |  |

**Returns:** void

## setStatus(status)
Set the websocket's status.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| status | [WebsocketStatus](enums/WebsocketStatus) | The status to set. | false |  |

**Returns:** void

## terminate()
Terminate the websocket. Does not notify the gateway
that you've disconnected. Should only be used when
the gateway won't respond (e.g. timeouts).

**Returns:** void

## unpack(data, type?)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |
| type | string |  | true |  |

**Returns:** any

