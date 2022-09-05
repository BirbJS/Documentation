---
layout: default
title: "Birb"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / Birb

# Class: Birb

## Hierarchy

- [`EventDispatcher`](../EventDispatcher/index.md)<[`BirbEvent`](../modules.md#birbevent)\>

  ↳ **`Birb`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [baseApiUrl](index.md#baseapiurl)
- [guilds](index.md#guilds)
- [intents](index.md#intents)
- [options](index.md#options)
- [ping](index.md#ping)
- [users](index.md#users)
- [ws](index.md#ws)

### Methods

- [clear](index.md#clear)
- [fly](index.md#fly)
- [getToken](index.md#gettoken)
- [setToken](index.md#settoken)
- [when](index.md#when)

## Constructors

### constructor

• **new Birb**(`options`)

Your journey starts here! :D

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`BirbOptions`](../modules.md#birboptions) | The options to initialize the Birb with. |

#### Overrides

[EventDispatcher](../EventDispatcher/index.md).[constructor](../EventDispatcher/index.md#constructor)

#### Defined in

src/classes/Birb.ts:51

## Properties

### baseApiUrl

• `Readonly` **baseApiUrl**: `string` = `'https://discord.com/api/v10'`

The base URL for API requests.

#### Defined in

src/classes/Birb.ts:22

___

### guilds

• **guilds**: [`GuildsManager`](../GuildsManager/index.md)

The guilds manager.

#### Defined in

src/classes/Birb.ts:40

___

### intents

• `Readonly` **intents**: [`Intents`](../Intents/index.md)

The Intents Bitfield the client was initialized with.

#### Defined in

src/classes/Birb.ts:18

___

### options

• `Readonly` **options**: [`BirbOptions`](../modules.md#birboptions)

The options passed to the Birb constructor.

#### Defined in

src/classes/Birb.ts:14

___

### ping

• **ping**: `number` = `0`

The current websocket latency to Discord, in milliseconds.

#### Defined in

src/classes/Birb.ts:36

___

### users

• **users**: [`UsersManager`](../UsersManager/index.md)

The users manager.

#### Defined in

src/classes/Birb.ts:44

___

### ws

• **ws**: [`Websocket`](../Websocket/index.md)

The websocket for the client.

#### Defined in

src/classes/Birb.ts:26

## Methods

### clear

▸ **clear**(): `void`

#### Returns

`void`

#### Inherited from

[EventDispatcher](../EventDispatcher/index.md).[clear](../EventDispatcher/index.md#clear)

#### Defined in

src/classes/EventDispatcher.ts:35

___

### fly

▸ **fly**(): `Promise`<[`Birb`](index.md)\>

#### Returns

`Promise`<[`Birb`](index.md)\>

#### Defined in

src/classes/Birb.ts:72

___

### getToken

▸ **getToken**(): `undefined` \| `string`

Seriously though, **don't share your bot's token** with anyone!

#### Returns

`undefined` \| `string`

#### Defined in

src/classes/Birb.ts:100

___

### setToken

▸ **setToken**(`token`): [`Birb`](index.md)

Sets the token.

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | `string` |

#### Returns

[`Birb`](index.md)

#### Defined in

src/classes/Birb.ts:92

___

### when

▸ **when**(`event`): [`EventListener`](../EventListener/index.md)<[`BirbEvent`](../modules.md#birbevent), `Function`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | [`BirbEvent`](../modules.md#birbevent) |

#### Returns

[`EventListener`](../EventListener/index.md)<[`BirbEvent`](../modules.md#birbevent), `Function`\>

#### Inherited from

[EventDispatcher](../EventDispatcher/index.md).[when](../EventDispatcher/index.md#when)

#### Defined in

src/classes/EventDispatcher.ts:14