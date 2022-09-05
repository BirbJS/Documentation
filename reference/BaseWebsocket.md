---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / BaseWebsocket

# Class: BaseWebsocket

## Hierarchy

- **`BaseWebsocket`**

  ↳ [`Websocket`](Websocket.md)

## Table of contents

### Constructors

- [constructor](BaseWebsocket.md#constructor)

### Properties

- [buffer](BaseWebsocket.md#buffer)
- [client](BaseWebsocket.md#client)
- [domain](BaseWebsocket.md#domain)
- [encoding](BaseWebsocket.md#encoding)
- [status](BaseWebsocket.md#status)
- [url](BaseWebsocket.md#url)

### Methods

- [generateURL](BaseWebsocket.md#generateurl)
- [init](BaseWebsocket.md#init)
- [pack](BaseWebsocket.md#pack)
- [processPacket](BaseWebsocket.md#processpacket)
- [unpack](BaseWebsocket.md#unpack)

## Constructors

### constructor

• **new BaseWebsocket**(`client`, `domain`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `domain` | `string` |

#### Defined in

src/classes/ws/BaseWebsocket.ts:46

## Properties

### buffer

• `Protected` **buffer**: `any`

The internal erlpack buffer.

#### Defined in

src/classes/ws/BaseWebsocket.ts:44

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Defined in

src/classes/ws/BaseWebsocket.ts:24

___

### domain

• **domain**: `string`

The websocket domain to connect to.

#### Defined in

src/classes/ws/BaseWebsocket.ts:28

___

### encoding

• **encoding**: `string`

The encoding to use.

#### Defined in

src/classes/ws/BaseWebsocket.ts:40

___

### status

• **status**: [`GatewayStatus`](GatewayStatus.md) = `Status.IDLE`

The current websocket status.

#### Defined in

src/classes/ws/BaseWebsocket.ts:36

___

### url

• **url**: [`URL`]( https://developer.mozilla.org/en-US/docs/Web/API/URL )

The URL to connect to.

#### Defined in

src/classes/ws/BaseWebsocket.ts:32

## Methods

### generateURL

▸ **generateURL**(): [`URL`]( https://developer.mozilla.org/en-US/docs/Web/API/URL )

#### Returns

[`URL`]( https://developer.mozilla.org/en-US/docs/Web/API/URL )

#### Defined in

src/classes/ws/BaseWebsocket.ts:151

___

### init

▸ `Protected` **init**(): `void`

Initializes ZLib if supported.

#### Returns

`void`

Voids once ZLib is initialized.

#### Defined in

src/classes/ws/BaseWebsocket.ts:142

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

#### Defined in

src/classes/ws/BaseWebsocket.ts:132

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

#### Defined in

src/classes/ws/BaseWebsocket.ts:63

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

#### Defined in

src/classes/ws/BaseWebsocket.ts:109
