---
layout: default
title: "GuildMember"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / GuildMember

# Class: GuildMember

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [avatarHash](index.md#avatarhash)
- [client](index.md#client)
- [guild](index.md#guild)
- [id](index.md#id)
- [joinedAt](index.md#joinedat)
- [nickname](index.md#nickname)
- [nitroBoostingSince](index.md#nitroboostingsince)
- [pendingMembershipScreening](index.md#pendingmembershipscreening)
- [roles](index.md#roles)
- [timedOutUntil](index.md#timedoutuntil)
- [user](index.md#user)
- [voiceDeafened](index.md#voicedeafened)
- [voiceMuted](index.md#voicemuted)

## Constructors

### constructor

• **new GuildMember**(`client`, `guild`, `member`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |
| `guild` | [`Guild`](../Guild/index.md) |
| `member` | [`APIGuildMemberWithUser`](../modules.md#apiguildmemberwithuser) |

#### Defined in

src/classes/GuildMember.ts:21

## Properties

### avatarHash

• **avatarHash**: ``null`` \| `string` = `null`

#### Defined in

src/classes/GuildMember.ts:12

___

### client

• **client**: [`Birb`](../Birb/index.md)

#### Defined in

src/classes/GuildMember.ts:7

___

### guild

• **guild**: [`Guild`](../Guild/index.md)

#### Defined in

src/classes/GuildMember.ts:8

___

### id

• `Readonly` **id**: `string`

#### Defined in

src/classes/GuildMember.ts:10

___

### joinedAt

• `Readonly` **joinedAt**: [`Date`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date )

#### Defined in

src/classes/GuildMember.ts:14

___

### nickname

• **nickname**: ``null`` \| `string` = `null`

#### Defined in

src/classes/GuildMember.ts:11

___

### nitroBoostingSince

• **nitroBoostingSince**: ``null`` \| [`Date`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date ) = `null`

#### Defined in

src/classes/GuildMember.ts:15

___

### pendingMembershipScreening

• **pendingMembershipScreening**: `boolean` = `false`

#### Defined in

src/classes/GuildMember.ts:18

___

### roles

• **roles**: `any`[]

#### Defined in

src/classes/GuildMember.ts:13

___

### timedOutUntil

• **timedOutUntil**: ``null`` \| [`Date`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date ) = `null`

#### Defined in

src/classes/GuildMember.ts:19

___

### user

• **user**: [`User`](../User/index.md)

#### Defined in

src/classes/GuildMember.ts:9

___

### voiceDeafened

• **voiceDeafened**: `boolean`

#### Defined in

src/classes/GuildMember.ts:16

___

### voiceMuted

• **voiceMuted**: `boolean`

#### Defined in

src/classes/GuildMember.ts:17
