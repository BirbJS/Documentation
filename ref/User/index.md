---
layout: default
title: "User"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / User

# Class: User

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [avatarHash](index.md#avatarhash)
- [bannerHash](index.md#bannerhash)
- [bot](index.md#bot)
- [client](index.md#client)
- [discriminator](index.md#discriminator)
- [flags](index.md#flags)
- [id](index.md#id)
- [system](index.md#system)
- [tag](index.md#tag)
- [username](index.md#username)

### Methods

- [isAutomated](index.md#isautomated)
- [toString](index.md#tostring)

## Constructors

### constructor

• **new User**(`client`, `user`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |
| `user` | [`APIUser`](../modules.md#apiuser) |

#### Defined in

src/classes/User.ts:47

## Properties

### avatarHash

• **avatarHash**: `undefined` \| ``null`` \| `string`

The user's avatar hash

#### Defined in

src/classes/User.ts:29

___

### bannerHash

• `Optional` **bannerHash**: ``null`` \| `string`

The user's banner hash

#### Defined in

src/classes/User.ts:41

___

### bot

• **bot**: `boolean` = `false`

Whether or not the user is a bot account

#### Defined in

src/classes/User.ts:33

___

### client

• **client**: [`Birb`](../Birb/index.md)

The Birb client

#### Defined in

src/classes/User.ts:9

___

### discriminator

• **discriminator**: `string`

The user's discriminator (Username#**0000**)

#### Defined in

src/classes/User.ts:21

___

### flags

• `Optional` **flags**: [`UserFlags`](../UserFlags/index.md)

The flags that are added to the user's account

#### Defined in

src/classes/User.ts:45

___

### id

• `Readonly` **id**: `string`

The user's ID (snowflake) as a string

#### Defined in

src/classes/User.ts:13

___

### system

• **system**: `boolean` = `false`

Whether or not the user is a part of the [Discord Urgent Message System](https://support.discord.com/hc/en-us/articles/360036118732-Discord-System-Messages)

#### Defined in

src/classes/User.ts:37

___

### tag

• **tag**: `string`

The user's tag (**Username#0000**)

#### Defined in

src/classes/User.ts:25

___

### username

• **username**: `string`

The user's username (**Username**#0000)

#### Defined in

src/classes/User.ts:17

## Methods

### isAutomated

▸ **isAutomated**(): `boolean`

#### Returns

`boolean`

`true` if the user is automated, `false` otherwise.

#### Defined in

src/classes/User.ts:88

___

### toString

▸ **toString**(): `string`

#### Returns

`string`

#### Defined in

src/classes/User.ts:92
