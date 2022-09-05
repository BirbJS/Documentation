---
layout: default
title: "Manager"
parent: "1"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / Manager

# Class: Manager<Type\>

## Type parameters

| Name |
| :------ |
| `Type` |

## Hierarchy

- **`Manager`**

  ↳ [`GuildMemberManager`](../GuildMemberManager/index.md)

  ↳ [`GuildsManager`](../GuildsManager/index.md)

  ↳ [`UsersManager`](../UsersManager/index.md)

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [cache](index.md#cache)
- [client](index.md#client)

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
| `client` | [`Birb`](../Birb/index.md) |

#### Defined in

src/classes/managers/Manager.ts:14

## Properties

### cache

• **cache**: [`Cache`](../Cache/index.md)<`string`, `Type`\>

The cache that contains all the Manager's items.

#### Defined in

src/classes/managers/Manager.ts:12

___

### client

• **client**: [`Birb`](../Birb/index.md)

The Birb client.

#### Defined in

src/classes/managers/Manager.ts:8
