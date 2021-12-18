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
| client | [Client](/classes/Client) | The client. | false | *none* |
| domain | string | The domain to connect to.
 | false | *none* |

# Properties
## buffer
{: .d-inline-block }

PROTECTED
{: .label .label-red }

The internal erlpack buffer.

**Type:** any

## client
The client that owns this websocket.

**Type:** [Client](/classes/Client)

## domain
The current Discord gateway URL.

**Type:** string

## encoding
The type of encoding to use. If `erlpack` is
installed (`npm install erlpack`), `etf` encoding
will be used. Otherwise, normal `json` encoding will
be used.

**Type:** string

## expectedGuilds
The guild IDs that the client is expecting to
receive from the Discord gateway.

**Type:** Set<string>

## heartbeatInterval
The interval to send heartbeats.

**Type:** Object | number

## lastHeartbeat
The time the last heartbeat was sent.

**Type:** number

## lastHeartbeatAcked
Whether or not the last heartbeat was acknowledged
by the Discord gateway.

**Type:** boolean

## lastResume
The time the last resume packet was sent.

**Type:** number

## lastSequenceIdentifier
The last sequence identifier received from the
Discord gateway.

**Type:** Object | number

## latency
The current latency (in milliseconds) between the
client and the Discord gateway.

**Type:** number

## schedulerLoop
The websocket's scheduler loop.

**Type:** Object | Timer

## sessionIdentifier
The session identifier from the Discord gateway.

**Type:** Object | string

## status
The current status of the websocket.

**Type:** [WebsocketStatus](/enums/WebsocketStatus)

## url
The websocket's currently set URL.

**Type:** URL

## ws
The websocket instance from the `ws` package.

**Type:** WebSocket

# Methods
## close(code?)
Close the websocket.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| code | number |   | true | *none* |

**Returns:** void

## connect()
Connect to the gateway.

**Returns:** void

## generateURL()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Generates the gateway URL.

**Returns:** URL

## heartbeat()
Send a heartbeat to the gateway.

**Returns:** Promise<void>

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Initializes ZLib if supported.

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

## pack(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Packs data for sending to Discord. If the encoding
is set to `etf`, this method will use the
`zlib-sync` (`npm install zlib-sync`) library to
pack its `etf` data. Otherwise, parses the JSON data
to a string.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to pack. | false | *none* |

**Returns:** any

## preventReconnect(value?)
Prevent reconnection.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| value | boolean |   | true | *none* |

**Returns:** void

## processPacket(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Attempts to process a packet by using ZLib to let
Discord send packets in chunks. If ZLib is not yet
installed (`npm install zlib-sync`), this method
will just pass the data through for unpacking
(`this.unpack()`).

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The packet's data. | false | *none* |

**Returns:** any

## reconnect()
Reconnect to the gateway.

**Returns:** void

## send(data)
Send a packet to the gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object | The data to send. | false | *none* |

**Returns:** void

## setSessionIdentifier(sessionIdentifier)
Set the websocket's session identifier.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| sessionIdentifier | string | The session identifier to set. | false | *none* |

**Returns:** void

## setStatus(status)
Set the websocket's status.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| status | [WebsocketStatus](/enums/WebsocketStatus) | The status to set. | false | *none* |

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

Unpacks a packet using the current encoding. If the
encoding is set to `etf`, this method will use the
`zlib-sync` (`npm install zlib-sync`) library to
unpack its `etf` data. Otherwise, parses the data to
normal JSON.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The packet's data. | false | *none* |
| type | string |   | true | *none* |

**Returns:** any

