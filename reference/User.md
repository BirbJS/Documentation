---
layout: default
title: User
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / User

# Class: User

## Table of contents

### Constructors

- [constructor](User.md#constructor)

### Properties

- [avatarHash](User.md#avatarhash)
- [bannerHash](User.md#bannerhash)
- [bot](User.md#bot)
- [client](User.md#client)
- [discriminator](User.md#discriminator)
- [flags](User.md#flags)
- [id](User.md#id)
- [system](User.md#system)
- [tag](User.md#tag)
- [username](User.md#username)

### Methods

- [isAutomated](User.md#isautomated)
- [toString](User.md#tostring)

## Constructors

### constructor

• **new User**(`client`, `user`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `user` | [`APIUser`](modules.md#apiuser) |

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

• **client**: [`Birb`](Birb.md)

The Birb client

#### Defined in

src/classes/User.ts:9

___

### discriminator

• **discriminator**: `string`

The user's discriminator (e.g. Username#**0000**)

#### Defined in

src/classes/User.ts:21

___

### flags

• `Optional` **flags**: [`UserFlags`](UserFlags.md)

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

The user's tag (e.g. **Username#0000**)

#### Defined in

src/classes/User.ts:25

___

### username

• **username**: `string`

The user's username (e.g. **Username**#0000)

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
