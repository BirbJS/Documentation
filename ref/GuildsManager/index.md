---
layout: default
title: "GuildsManager"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / GuildsManager

# Class: GuildsManager

## Hierarchy

- [`Manager`](../Manager/index.md)<[`Guild`](../Guild/index.md)\>

  ↳ **`GuildsManager`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [cache](index.md#cache)
- [client](index.md#client)
- [unavailableCache](index.md#unavailablecache)

### Methods

- [fetch](index.md#fetch)
- [resolve](index.md#resolve)
- [total](index.md#total)

## Constructors

### constructor

• **new GuildsManager**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |

#### Overrides

[Manager](../Manager/index.md).[constructor](../Manager/index.md#constructor)

#### Defined in

src/classes/managers/GuildsManager.ts:23

## Properties

### cache

• **cache**: [`Cache`](../Cache/index.md)<`string`, [`Guild`](../Guild/index.md)\>

The cache for guilds. This cache includes guilds that are available and unavailable.
For a guild to be stored in this cache, the client must see it available at least once.

#### Overrides

[Manager](../Manager/index.md).[cache](../Manager/index.md#cache)

#### Defined in

src/classes/managers/GuildsManager.ts:15

___

### client

• **client**: [`Birb`](../Birb/index.md)

The Birb client.

#### Inherited from

[Manager](../Manager/index.md).[client](../Manager/index.md#client)

#### Defined in

src/classes/managers/Manager.ts:8

___

### unavailableCache

• **unavailableCache**: [`Cache`](../Cache/index.md)<`string`, [`GuildPartial`](../GuildPartial/index.md)\>

The cache for **unavailable guilds**. Guilds are pushed here when they are unavailable
and the client has never seen them available. This allows you to keep track of these
guilds, but they won't unintentionally get in the way.

#### Defined in

src/classes/managers/GuildsManager.ts:21

## Methods

### fetch

▸ **fetch**(`target`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](../Guild/index.md)\>

Fetch a guild from the cache, or the API if it is not cached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildPartial`](../GuildPartial/index.md) \| [`Guild`](../Guild/index.md) | The target guild. |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](../Guild/index.md)\>

#### Defined in

src/classes/managers/GuildsManager.ts:56

___

### resolve

▸ **resolve**(`target`): `undefined` \| [`GuildPartial`](../GuildPartial/index.md) \| [`Guild`](../Guild/index.md)

Resolves a guild in the cache from an ID.

**Note:** This method will not fetch the guild from the API, and will check
both caches (available and unavailable). To fetch directly from the API, use the
`fetch()` method. To get from the available cache only, use the `get()` method on
the `cache` property (e.g. `guilds.cache.get()`).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildPartial`](../GuildPartial/index.md) \| [`Guild`](../Guild/index.md) | The ID guild. |

#### Returns

`undefined` \| [`GuildPartial`](../GuildPartial/index.md) \| [`Guild`](../Guild/index.md)

The Guild if available, otherwise a GuildPartial. Returns `undefined` if the guild is not cached.

#### Defined in

src/classes/managers/GuildsManager.ts:40

___

### total

▸ **total**(): `number`

#### Returns

`number`

The total amount of guilds the client is in.

#### Defined in

src/classes/managers/GuildsManager.ts:94
