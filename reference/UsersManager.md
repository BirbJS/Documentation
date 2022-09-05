---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / UsersManager

# Class: UsersManager

## Hierarchy

- [`Manager`](Manager.md)<[`User`](User.md)\>

  ↳ **`UsersManager`**

## Table of contents

### Constructors

- [constructor](UsersManager.md#constructor)

### Properties

- [cache](UsersManager.md#cache)
- [client](UsersManager.md#client)

### Methods

- [fetch](UsersManager.md#fetch)
- [resolve](UsersManager.md#resolve)
- [total](UsersManager.md#total)

## Constructors

### constructor

• **new UsersManager**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |

#### Overrides

[Manager](Manager.md).[constructor](Manager.md#constructor)

#### Defined in

src/classes/managers/UsersManager.ts:9

## Properties

### cache

• **cache**: [`Cache`](Cache.md)<`string`, [`User`](User.md)\>

The cache that contains all the Manager's items.

#### Inherited from

[Manager](Manager.md).[cache](Manager.md#cache)

#### Defined in

src/classes/managers/Manager.ts:12

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Inherited from

[Manager](Manager.md).[client](Manager.md#client)

#### Defined in

src/classes/managers/Manager.ts:8

## Methods

### fetch

▸ **fetch**(`target`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](Guild.md)\>

Fetch a user from the cache, or the API if it is not cached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildPartial`](GuildPartial.md) \| [`Guild`](Guild.md) | The target user. |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](Guild.md)\>

#### Defined in

src/classes/managers/UsersManager.ts:25

___

### resolve

▸ **resolve**(`target`): `undefined` \| [`User`](User.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `string` \| [`User`](User.md) |

#### Returns

`undefined` \| [`User`](User.md)

#### Defined in

src/classes/managers/UsersManager.ts:13

___

### total

▸ **total**(): `number`

#### Returns

`number`

The total amount of users cached in this manager.

#### Defined in

src/classes/managers/UsersManager.ts:34
