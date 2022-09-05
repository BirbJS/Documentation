---
layout: default
title: "GuildPartial"
parent: "1"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / GuildPartial

# Class: GuildPartial

## Hierarchy

- **`GuildPartial`**

  ↳ [`Guild`](../Guild/index.md)

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [available](index.md#available)
- [client](index.md#client)
- [id](index.md#id)

### Methods

- [fetch](index.md#fetch)
- [isPartial](index.md#ispartial)

## Constructors

### constructor

• **new GuildPartial**(`client`, `guild`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |
| `guild` | [`APIGuild`](../modules.md#apiguild) \| [`APIGuildPartial`](../modules.md#apiguildpartial) |

#### Defined in

src/classes/GuildPartial.ts:12

## Properties

### available

• **available**: `boolean` = `false`

#### Defined in

src/classes/GuildPartial.ts:10

___

### client

• **client**: [`Birb`](../Birb/index.md)

#### Defined in

src/classes/GuildPartial.ts:8

___

### id

• `Readonly` **id**: `string`

#### Defined in

src/classes/GuildPartial.ts:9

## Methods

### fetch

▸ **fetch**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](../Guild/index.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](../Guild/index.md)\>

#### Defined in

src/classes/GuildPartial.ts:25

___

### isPartial

▸ **isPartial**(): `boolean`

#### Returns

`boolean`

`true` if this is a partial guild, `false` otherwise.

#### Defined in

src/classes/GuildPartial.ts:49
