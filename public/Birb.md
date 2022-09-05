---
layout: default
title: "Birb"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / Birb

# Class: Birb

## Hierarchy

- [`EventDispatcher`](EventDispatcher.md)<[`BirbEvent`](modules.md#birbevent)\>

  ↳ **`Birb`**

## Table of contents

### Constructors

- [constructor](Birb.md#constructor)

### Properties

- [baseApiUrl](Birb.md#baseapiurl)
- [guilds](Birb.md#guilds)
- [intents](Birb.md#intents)
- [options](Birb.md#options)
- [ping](Birb.md#ping)
- [users](Birb.md#users)
- [ws](Birb.md#ws)

### Methods

- [clear](Birb.md#clear)
- [fly](Birb.md#fly)
- [getToken](Birb.md#gettoken)
- [setToken](Birb.md#settoken)
- [when](Birb.md#when)

## Constructors

### constructor

• **new Birb**(`options`)

Your journey starts here! :D

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`BirbOptions`](modules.md#birboptions) | The options to initialize the Birb with. |

#### Overrides

[EventDispatcher](EventDispatcher.md).[constructor](EventDispatcher.md#constructor)

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

• **guilds**: [`GuildsManager`](GuildsManager.md)

The guilds manager.

#### Defined in

src/classes/Birb.ts:40

___

### intents

• `Readonly` **intents**: [`Intents`](Intents.md)

The Intents Bitfield the client was initialized with.

#### Defined in

src/classes/Birb.ts:18

___

### options

• `Readonly` **options**: [`BirbOptions`](modules.md#birboptions)

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

• **users**: [`UsersManager`](UsersManager.md)

The users manager.

#### Defined in

src/classes/Birb.ts:44

___

### ws

• **ws**: [`Websocket`](Websocket.md)

The websocket for the client.

#### Defined in

src/classes/Birb.ts:26

## Methods

### clear

▸ **clear**(): `void`

#### Returns

`void`

#### Inherited from

[EventDispatcher](EventDispatcher.md).[clear](EventDispatcher.md#clear)

#### Defined in

src/classes/EventDispatcher.ts:35

___

### fly

▸ **fly**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Birb`](Birb.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Birb`](Birb.md)\>

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

▸ **setToken**(`token`): [`Birb`](Birb.md)

Sets the token.

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | `string` |

#### Returns

[`Birb`](Birb.md)

#### Defined in

src/classes/Birb.ts:92

___

### when

▸ **when**(`event`): [`EventListener`](EventListener.md)<[`BirbEvent`](modules.md#birbevent), [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function )\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | [`BirbEvent`](modules.md#birbevent) |

#### Returns

[`EventListener`](EventListener.md)<[`BirbEvent`](modules.md#birbevent), [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function )\>

#### Inherited from

[EventDispatcher](EventDispatcher.md).[when](EventDispatcher.md#when)

#### Defined in

src/classes/EventDispatcher.ts:14
