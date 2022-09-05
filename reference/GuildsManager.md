---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / GuildsManager

# Class: GuildsManager

## Hierarchy

- [`Manager`](Manager.md)<[`Guild`](Guild.md)\>

  ↳ **`GuildsManager`**

## Table of contents

### Constructors

- [constructor](GuildsManager.md#constructor)

### Properties

- [cache](GuildsManager.md#cache)
- [client](GuildsManager.md#client)
- [unavailableCache](GuildsManager.md#unavailablecache)

### Methods

- [fetch](GuildsManager.md#fetch)
- [resolve](GuildsManager.md#resolve)
- [total](GuildsManager.md#total)

## Constructors

### constructor

• **new GuildsManager**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |

#### Overrides

[Manager](Manager.md).[constructor](Manager.md#constructor)

#### Defined in

src/classes/managers/GuildsManager.ts:23

## Properties

### cache

• **cache**: [`Cache`](Cache.md)<`string`, [`Guild`](Guild.md)\>

The cache for guilds. This cache includes guilds that are available and unavailable.
For a guild to be stored in this cache, the client must see it available at least once.

#### Overrides

[Manager](Manager.md).[cache](Manager.md#cache)

#### Defined in

src/classes/managers/GuildsManager.ts:15

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Inherited from

[Manager](Manager.md).[client](Manager.md#client)

#### Defined in

src/classes/managers/Manager.ts:8

___

### unavailableCache

• **unavailableCache**: [`Cache`](Cache.md)<`string`, [`GuildPartial`](GuildPartial.md)\>

The cache for **unavailable guilds**. Guilds are pushed here when they are unavailable
and the client has never seen them available. This allows you to keep track of these
guilds, but they won't unintentionally get in the way.

#### Defined in

src/classes/managers/GuildsManager.ts:21

## Methods

### fetch

▸ **fetch**(`target`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](Guild.md)\>

Fetch a guild from the cache, or the API if it is not cached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildPartial`](GuildPartial.md) \| [`Guild`](Guild.md) | The target guild. |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](Guild.md)\>

#### Defined in

src/classes/managers/GuildsManager.ts:56

___

### resolve

▸ **resolve**(`target`): `undefined` \| [`GuildPartial`](GuildPartial.md) \| [`Guild`](Guild.md)

Resolves a guild in the cache from an ID.

**Note:** This method will not fetch the guild from the API, and will check
both caches (available and unavailable). To fetch directly from the API, use the
`fetch()` method. To get from the available cache only, use the `get()` method on
the `cache` property (e.g. `guilds.cache.get()`).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildPartial`](GuildPartial.md) \| [`Guild`](Guild.md) | The ID guild. |

#### Returns

`undefined` \| [`GuildPartial`](GuildPartial.md) \| [`Guild`](Guild.md)

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
