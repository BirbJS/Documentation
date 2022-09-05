---
layout: default
title: "GuildMemberManager"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / GuildMemberManager

# Class: GuildMemberManager

## Hierarchy

- [`Manager`](../Manager/index.md)<[`GuildMember`](../GuildMember/index.md)\>

  ↳ **`GuildMemberManager`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [cache](index.md#cache)
- [client](index.md#client)
- [guild](index.md#guild)

### Methods

- [fetch](index.md#fetch)
- [resolve](index.md#resolve)
- [total](index.md#total)

## Constructors

### constructor

• **new GuildMemberManager**(`client`, `guild`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |
| `guild` | [`Guild`](../Guild/index.md) |

#### Overrides

[Manager](../Manager/index.md).[constructor](../Manager/index.md#constructor)

#### Defined in

src/classes/managers/GuildMembersManager.ts:13

## Properties

### cache

• **cache**: [`Cache`](../Cache/index.md)<`string`, [`GuildMember`](../GuildMember/index.md)\>

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

___

### guild

• **guild**: [`Guild`](../Guild/index.md)

The parent Guild.

#### Defined in

src/classes/managers/GuildMembersManager.ts:11

## Methods

### fetch

▸ **fetch**(`target`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`GuildMember`](../GuildMember/index.md)\>

Fetch a guild from the cache, or the API if it is not cached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildMember`](../GuildMember/index.md) | The target member. |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`GuildMember`](../GuildMember/index.md)\>

#### Defined in

src/classes/managers/GuildMembersManager.ts:27

___

### resolve

▸ **resolve**(`target`): `undefined` \| [`GuildMember`](../GuildMember/index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `string` \| [`GuildMember`](../GuildMember/index.md) |

#### Returns

`undefined` \| [`GuildMember`](../GuildMember/index.md)

#### Defined in

src/classes/managers/GuildMembersManager.ts:18

___

### total

▸ **total**(): `number`

#### Returns

`number`

The total amount of members cached in this manager. There may be more or less members in the guild.

#### Defined in

src/classes/managers/GuildMembersManager.ts:36
