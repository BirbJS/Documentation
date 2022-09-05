---
layout: default
title: "Websocket"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / Websocket

# Class: Websocket

## Hierarchy

- [`BaseWebsocket`](BaseWebsocket.md)

  ↳ **`Websocket`**

## Table of contents

### Constructors

- [constructor](Websocket.md#constructor)

### Properties

- [buffer](Websocket.md#buffer)
- [client](Websocket.md#client)
- [connectedSince](Websocket.md#connectedsince)
- [doNotReconnect](Websocket.md#donotreconnect)
- [domain](Websocket.md#domain)
- [encoding](Websocket.md#encoding)
- [expectedGuilds](Websocket.md#expectedguilds)
- [hasBeenReady](Websocket.md#hasbeenready)
- [heartbeatInterval](Websocket.md#heartbeatinterval)
- [lastHeartbeat](Websocket.md#lastheartbeat)
- [lastHeartbeatAcked](Websocket.md#lastheartbeatacked)
- [lastResume](Websocket.md#lastresume)
- [lastSequenceIdentifier](Websocket.md#lastsequenceidentifier)
- [ping](Websocket.md#ping)
- [resumeGatewayUrl](Websocket.md#resumegatewayurl)
- [schedulerLoop](Websocket.md#schedulerloop)
- [sessionIdentifier](Websocket.md#sessionidentifier)
- [socket](Websocket.md#socket)
- [status](Websocket.md#status)
- [url](Websocket.md#url)

### Methods

- [close](Websocket.md#close)
- [connect](Websocket.md#connect)
- [generateURL](Websocket.md#generateurl)
- [heartbeat](Websocket.md#heartbeat)
- [init](Websocket.md#init)
- [isClosed](Websocket.md#isclosed)
- [isConnected](Websocket.md#isconnected)
- [isConnecting](Websocket.md#isconnecting)
- [pack](Websocket.md#pack)
- [preventReconnect](Websocket.md#preventreconnect)
- [processPacket](Websocket.md#processpacket)
- [reconnect](Websocket.md#reconnect)
- [send](Websocket.md#send)
- [setSessionIdentifier](Websocket.md#setsessionidentifier)
- [setStatus](Websocket.md#setstatus)
- [terminate](Websocket.md#terminate)
- [unpack](Websocket.md#unpack)

## Constructors

### constructor

• **new Websocket**(`client`, `domain`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `domain` | `string` |

#### Overrides

[BaseWebsocket](BaseWebsocket.md).[constructor](BaseWebsocket.md#constructor)

#### Defined in

src/classes/ws/Websocket.ts:66

## Properties

### buffer

• `Protected` **buffer**: `any`

The internal erlpack buffer.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[buffer](BaseWebsocket.md#buffer)

#### Defined in

src/classes/ws/BaseWebsocket.ts:44

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[client](BaseWebsocket.md#client)

#### Defined in

src/classes/ws/BaseWebsocket.ts:24

___

### connectedSince

• **connectedSince**: `number` = `0`

The time since the last connection.

#### Defined in

src/classes/ws/Websocket.ts:55

___

### doNotReconnect

• **doNotReconnect**: `boolean` = `false`

Whether or not to prevent reconnection.

#### Defined in

src/classes/ws/Websocket.ts:47

___

### domain

• **domain**: `string`

The websocket domain to connect to.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[domain](BaseWebsocket.md#domain)

#### Defined in

src/classes/ws/BaseWebsocket.ts:28

___

### encoding

• **encoding**: `string`

The encoding to use.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[encoding](BaseWebsocket.md#encoding)

#### Defined in

src/classes/ws/BaseWebsocket.ts:40

___

### expectedGuilds

• **expectedGuilds**: `string`[] = `[]`

The guild IDs we are expecting to receive.

#### Defined in

src/classes/ws/Websocket.ts:63

___

### hasBeenReady

• **hasBeenReady**: `boolean` = `false`

Whether or not the websocket has been ready before.

#### Defined in

src/classes/ws/Websocket.ts:59

___

### heartbeatInterval

• **heartbeatInterval**: `undefined` \| `number`

The interval to send heartbeats.

#### Defined in

src/classes/ws/Websocket.ts:30

___

### lastHeartbeat

• **lastHeartbeat**: `number` = `0`

The time the last heartbeat was sent.

#### Defined in

src/classes/ws/Websocket.ts:21

___

### lastHeartbeatAcked

• **lastHeartbeatAcked**: `boolean` = `false`

Whether or not the last heartbeat was acknowledged
by the Discord gateway.

#### Defined in

src/classes/ws/Websocket.ts:26

___

### lastResume

• **lastResume**: `number` = `0`

The time the last resume packet was sent.

#### Defined in

src/classes/ws/Websocket.ts:51

___

### lastSequenceIdentifier

• **lastSequenceIdentifier**: `undefined` \| `number`

The last sequence identifier received from the
Discord gateway.

#### Defined in

src/classes/ws/Websocket.ts:43

___

### ping

• **ping**: `number` = `0`

The current latency (in milliseconds) between the
client and the Discord gateway.

#### Defined in

src/classes/ws/Websocket.ts:17

___

### resumeGatewayUrl

• **resumeGatewayUrl**: `undefined` \| `string`

The URL to use when resuming a connection.

#### Defined in

src/classes/ws/Websocket.ts:38

___

### schedulerLoop

• **schedulerLoop**: `undefined` \| `Timer`

#### Defined in

src/classes/ws/Websocket.ts:64

___

### sessionIdentifier

• **sessionIdentifier**: `undefined` \| `string`

The session identifier from the Discord gateway.

#### Defined in

src/classes/ws/Websocket.ts:34

___

### socket

• **socket**: `undefined` \| `WebSocket`

The websocket instance from the `ws` package.

#### Defined in

src/classes/ws/Websocket.ts:12

___

### status

• **status**: [`GatewayStatus`](GatewayStatus.md) = `Status.IDLE`

The current websocket status.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[status](BaseWebsocket.md#status)

#### Defined in

src/classes/ws/BaseWebsocket.ts:36

___

### url

• **url**: [`URL`]( https://developer.mozilla.org/en-US/docs/Web/API/URL )

The URL to connect to.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[url](BaseWebsocket.md#url)

#### Defined in

src/classes/ws/BaseWebsocket.ts:32

## Methods

### close

▸ **close**(`code?`): `void`

Close the websocket.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `code?` | `number` | The close code. |

#### Returns

`void`

Voids once completed.

#### Defined in

src/classes/ws/Websocket.ts:509

___

### connect

▸ **connect**(): `void`

#### Returns

`void`

#### Defined in

src/classes/ws/Websocket.ts:70

___

### generateURL

▸ **generateURL**(): [`URL`]( https://developer.mozilla.org/en-US/docs/Web/API/URL )

#### Returns

[`URL`]( https://developer.mozilla.org/en-US/docs/Web/API/URL )

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[generateURL](BaseWebsocket.md#generateurl)

#### Defined in

src/classes/ws/BaseWebsocket.ts:151

___

### heartbeat

▸ **heartbeat**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`void`\>

Send a heartbeat to the gateway.

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`void`\>

Voids once sent.

#### Defined in

src/classes/ws/Websocket.ts:476

___

### init

▸ `Protected` **init**(): `void`

Initializes ZLib if supported.

#### Returns

`void`

Voids once ZLib is initialized.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[init](BaseWebsocket.md#init)

#### Defined in

src/classes/ws/BaseWebsocket.ts:142

___

### isClosed

▸ **isClosed**(): `boolean`

Check if the websocket is closed.

#### Returns

`boolean`

Whether or not the websocket is closed.

#### Defined in

src/classes/ws/Websocket.ts:568

___

### isConnected

▸ **isConnected**(): `boolean`

Check if the websocket is connected.

#### Returns

`boolean`

Whether or not the websocket is connected.

#### Defined in

src/classes/ws/Websocket.ts:545

___

### isConnecting

▸ **isConnecting**(): `boolean`

Check if the websocket is connecting.

#### Returns

`boolean`

Whether or not the websocket is connecting.

#### Defined in

src/classes/ws/Websocket.ts:559

___

### pack

▸ `Protected` **pack**(`data`): `any`

Packs data for sending to Discord. If the encoding
is set to `etf`, this method will use the
`zlib-sync` (`npm install zlib-sync`) library to
pack its `etf` data. Otherwise, parses the JSON data
to a string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any` | The data to pack. |

#### Returns

`any`

Hopefully, the data's packed form.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[pack](BaseWebsocket.md#pack)

#### Defined in

src/classes/ws/BaseWebsocket.ts:132

___

### preventReconnect

▸ **preventReconnect**(`value?`): `void`

Prevent reconnection.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`void`

Voids once completed.

#### Defined in

src/classes/ws/Websocket.ts:578

___

### processPacket

▸ `Protected` **processPacket**(`data`): `any`

Attempts to process a packet by using ZLib to let
Discord send packets in chunks. If ZLib is not yet
installed (`npm install zlib-sync`), this method
will just pass the data through for unpacking
(`this.unpack()`).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any` | The packet's data. |

#### Returns

`any`

Hopefully, the packet's JSON form.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[processPacket](BaseWebsocket.md#processpacket)

#### Defined in

src/classes/ws/BaseWebsocket.ts:63

___

### reconnect

▸ **reconnect**(): `void`

Reconnect to the gateway.

#### Returns

`void`

Voids once completed.

#### Defined in

src/classes/ws/Websocket.ts:89

___

### send

▸ **send**(`data`): `void`

Send a packet to the gateway.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Object`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object ) | The data to send. |

#### Returns

`void`

Voids once sent.

#### Defined in

src/classes/ws/Websocket.ts:440

___

### setSessionIdentifier

▸ **setSessionIdentifier**(`sessionIdentifier`): `void`

Set the websocket's session identifier.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionIdentifier` | `string` | The session identifier to set. |

#### Returns

`void`

Voids once completed.

#### Defined in

src/classes/ws/Websocket.ts:598

___

### setStatus

▸ **setStatus**(`status`): `void`

Set the websocket's status.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `status` | [`GatewayStatus`](GatewayStatus.md) | The status to set. |

#### Returns

`void`

Voids once completed.

#### Defined in

src/classes/ws/Websocket.ts:588

___

### terminate

▸ **terminate**(): `void`

Terminate the websocket. Does not notify the gateway
that you've disconnected. Should only be used when
the gateway won't respond (e.g. timeouts).

#### Returns

`void`

Voids once completed.

#### Defined in

src/classes/ws/Websocket.ts:530

___

### unpack

▸ `Protected` **unpack**(`data`, `type?`): `any`

Unpacks a packet using the current encoding. If the
encoding is set to `etf`, this method will use the
`zlib-sync` (`npm install zlib-sync`) library to
unpack its `etf` data. Otherwise, parses the data to
normal JSON.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any` | The packet's data. |
| `type?` | `string` | The packet's encoding. |

#### Returns

`any`

Hopefully, the packet's JSON form.

#### Inherited from

[BaseWebsocket](BaseWebsocket.md).[unpack](BaseWebsocket.md#unpack)

#### Defined in

src/classes/ws/BaseWebsocket.ts:109
