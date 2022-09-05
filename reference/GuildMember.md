---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / GuildMember

# Class: GuildMember

## Table of contents

### Constructors

- [constructor](GuildMember.md#constructor)

### Properties

- [avatarHash](GuildMember.md#avatarhash)
- [client](GuildMember.md#client)
- [guild](GuildMember.md#guild)
- [id](GuildMember.md#id)
- [joinedAt](GuildMember.md#joinedat)
- [nickname](GuildMember.md#nickname)
- [nitroBoostingSince](GuildMember.md#nitroboostingsince)
- [pendingMembershipScreening](GuildMember.md#pendingmembershipscreening)
- [roles](GuildMember.md#roles)
- [timedOutUntil](GuildMember.md#timedoutuntil)
- [user](GuildMember.md#user)
- [voiceDeafened](GuildMember.md#voicedeafened)
- [voiceMuted](GuildMember.md#voicemuted)

## Constructors

### constructor

• **new GuildMember**(`client`, `guild`, `member`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `guild` | [`Guild`](Guild.md) |
| `member` | [`APIGuildMemberWithUser`](modules.md#apiguildmemberwithuser) |

#### Defined in

src/classes/GuildMember.ts:21

## Properties

### avatarHash

• **avatarHash**: ``null`` \| `string` = `null`

#### Defined in

src/classes/GuildMember.ts:12

___

### client

• **client**: [`Birb`](Birb.md)

#### Defined in

src/classes/GuildMember.ts:7

___

### guild

• **guild**: [`Guild`](Guild.md)

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

• **user**: [`User`](User.md)

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
