---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / GuildPartial

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

src/classes/GuildPartial.ts:23

## Properties

### available

• **available**: `boolean` = `false`

It is recommended to check if this value is `true` before performing actions
on the guild. If this value is `false`, the guild is unavailable due to a 
temporary Discord outage.

#### Defined in

src/classes/GuildPartial.ts:21

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client

#### Defined in

src/classes/GuildPartial.ts:11

___

### id

• `Readonly` **id**: `string`

The guild's ID (snowflake) as a string

#### Defined in

src/classes/GuildPartial.ts:15

## Methods

### fetch

▸ **fetch**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Defined in

src/classes/GuildPartial.ts:36

___

### isPartial

▸ **isPartial**(): `boolean`

#### Returns

`boolean`

`true` if this is a partial guild, `false` otherwise.

#### Defined in

src/classes/GuildPartial.ts:60
