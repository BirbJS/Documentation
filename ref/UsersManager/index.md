---
layout: default
title: "UsersManager"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / UsersManager

# Class: UsersManager

## Hierarchy

- [`Manager`](../Manager/index.md)<[`User`](../User/index.md)\>

  ↳ **`UsersManager`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [cache](index.md#cache)
- [client](index.md#client)

### Methods

- [fetch](index.md#fetch)
- [resolve](index.md#resolve)
- [total](index.md#total)

## Constructors

### constructor

• **new UsersManager**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |

#### Overrides

[Manager](../Manager/index.md).[constructor](../Manager/index.md#constructor)

#### Defined in

src/classes/managers/UsersManager.ts:9

## Properties

### cache

• **cache**: [`Cache`](../Cache/index.md)<`string`, [`User`](../User/index.md)\>

The cache that contains all the Manager's items.

#### Inherited from

[Manager](../Manager/index.md).[cache](../Manager/index.md#cache)

#### Defined in

src/classes/managers/Manager.ts:12

___

### client

• **client**: [`Birb`](../Birb/index.md)

The Birb client.

#### Inherited from

[Manager](../Manager/index.md).[client](../Manager/index.md#client)

#### Defined in

src/classes/managers/Manager.ts:8

## Methods

### fetch

▸ **fetch**(`target`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](../Guild/index.md)\>

Fetch a user from the cache, or the API if it is not cached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildPartial`](../GuildPartial/index.md) \| [`Guild`](../Guild/index.md) | The target user. |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`Guild`](../Guild/index.md)\>

#### Defined in

src/classes/managers/UsersManager.ts:25

___

### resolve

▸ **resolve**(`target`): `undefined` \| [`User`](../User/index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `string` \| [`User`](../User/index.md) |

#### Returns

`undefined` \| [`User`](../User/index.md)

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
