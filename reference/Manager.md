---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / Manager

# Class: Manager<Type\>

## Type parameters

| Name |
| :------ |
| `Type` |

## Hierarchy

- **`Manager`**

  ↳ [`GuildMemberManager`](GuildMemberManager.md)

  ↳ [`GuildsManager`](GuildsManager.md)

  ↳ [`UsersManager`](UsersManager.md)

## Table of contents

### Constructors

- [constructor](Manager.md#constructor)

### Properties

- [cache](Manager.md#cache)
- [client](Manager.md#client)

## Constructors

### constructor

• **new Manager**<`Type`\>(`client`)

#### Type parameters

| Name |
| :------ |
| `Type` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |

#### Defined in

src/classes/managers/Manager.ts:14

## Properties

### cache

• **cache**: [`Cache`](Cache.md)<`string`, `Type`\>

The cache that contains all the Manager's items.

#### Defined in

src/classes/managers/Manager.ts:12

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Defined in

src/classes/managers/Manager.ts:8
