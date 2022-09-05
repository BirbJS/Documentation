---
layout: default
title: "GuildPartial"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / GuildPartial

# Class: GuildPartial

## Hierarchy

- **`GuildPartial`**

  ↳ [`Guild`](Guild.md)

## Table of contents

### Constructors

- [constructor](GuildPartial.md#constructor)

### Properties

- [available](GuildPartial.md#available)
- [client](GuildPartial.md#client)
- [id](GuildPartial.md#id)

### Methods

- [fetch](GuildPartial.md#fetch)
- [isPartial](GuildPartial.md#ispartial)

## Constructors

### constructor

• **new GuildPartial**(`client`, `guild`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `guild` | [`APIGuild`](modules.md#apiguild) \| [`APIGuildPartial`](modules.md#apiguildpartial) |

#### Defined in

src/classes/GuildPartial.ts:12

## Properties

### available

• **available**: `boolean` = `false`

#### Defined in

src/classes/GuildPartial.ts:10

___

### client

• **client**: [`Birb`](Birb.md)

#### Defined in

src/classes/GuildPartial.ts:8

___

### id

• `Readonly` **id**: `string`

#### Defined in

src/classes/GuildPartial.ts:9

## Methods

### fetch

▸ **fetch**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

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
