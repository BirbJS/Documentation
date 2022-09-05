---
layout: default
title: GuildMemberManager
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / GuildMemberManager

# Class: GuildMemberManager

## Hierarchy

- [`Manager`](Manager.md)<[`GuildMember`](GuildMember.md)\>

  ↳ **`GuildMemberManager`**

## Table of contents

### Constructors

- [constructor](GuildMemberManager.md#constructor)

### Properties

- [cache](GuildMemberManager.md#cache)
- [client](GuildMemberManager.md#client)
- [guild](GuildMemberManager.md#guild)

### Methods

- [fetch](GuildMemberManager.md#fetch)
- [resolve](GuildMemberManager.md#resolve)
- [total](GuildMemberManager.md#total)

## Constructors

### constructor

• **new GuildMemberManager**(`client`, `guild`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `guild` | [`Guild`](Guild.md) |

#### Overrides

[Manager](Manager.md).[constructor](Manager.md#constructor)

#### Defined in

src/classes/managers/GuildMembersManager.ts:13

## Properties

### cache

• **cache**: [`Cache`](Cache.md)<`string`, [`GuildMember`](GuildMember.md)\>

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

___

### guild

• **guild**: [`Guild`](Guild.md)

The parent Guild.

#### Defined in

src/classes/managers/GuildMembersManager.ts:11

## Methods

### fetch

▸ **fetch**(`target`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`GuildMember`](GuildMember.md)\>

Fetch a guild from the cache, or the API if it is not cached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `string` \| [`GuildMember`](GuildMember.md) | The target member. |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<`undefined` \| [`GuildMember`](GuildMember.md)\>

#### Defined in

src/classes/managers/GuildMembersManager.ts:27

___

### resolve

▸ **resolve**(`target`): `undefined` \| [`GuildMember`](GuildMember.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `string` \| [`GuildMember`](GuildMember.md) |

#### Returns

`undefined` \| [`GuildMember`](GuildMember.md)

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
