---
layout: default
title: "Intents"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / Intents

# Class: Intents

## Hierarchy

- [`Bitfield`](Bitfield.md)<[`IntentsString`](modules.md#intentsstring)\>

  ↳ **`Intents`**

## Table of contents

### Constructors

- [constructor](Intents.md#constructor)

### Properties

- [bits](Intents.md#bits)
- [FLAGS](Intents.md#flags)

### Methods

- [add](Intents.md#add)
- [clone](Intents.md#clone)
- [convert](Intents.md#convert)
- [has](Intents.md#has)
- [isEmpty](Intents.md#isempty)
- [isLocked](Intents.md#islocked)
- [remove](Intents.md#remove)
- [set](Intents.md#set)
- [toArray](Intents.md#toarray)
- [toBigInt](Intents.md#tobigint)

## Constructors

### constructor

• **new Intents**(`bits?`)

The Intents Bitfield stores bits as bigints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bits?` | `number` \| `bigint` | The bigint or number representation of the Bitfield. |

#### Overrides

[Bitfield](Bitfield.md).[constructor](Bitfield.md#constructor)

#### Defined in

src/classes/bitfields/Intents.ts:38

## Properties

### bits

• **bits**: `bigint`

The bits as a bigint.

#### Inherited from

[Bitfield](Bitfield.md).[bits](Bitfield.md#bits)

#### Defined in

src/classes/bitfields/Bitfield.ts:10

___

### FLAGS

▪ `Static` `Readonly` **FLAGS**: `Object` = `IntentFlag`

The possible Intents the client can use.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `AUTO_MODERATION_CONFIGURATION` | `bigint` |
| `AUTO_MODERATION_EXECUTION` | `bigint` |
| `DIRECT_MESSAGES` | `bigint` |
| `DIRECT_MESSAGE_REACTIONS` | `bigint` |
| `DIRECT_MESSAGE_TYPING` | `bigint` |
| `GUILDS` | `bigint` |
| `GUILD_BANS` | `bigint` |
| `GUILD_EMOJIS_AND_STICKERS` | `bigint` |
| `GUILD_INTEGRATIONS` | `bigint` |
| `GUILD_INVITES` | `bigint` |
| `GUILD_MEMBERS` | `bigint` |
| `GUILD_MESSAGES` | `bigint` |
| `GUILD_MESSAGE_REACTIONS` | `bigint` |
| `GUILD_MESSAGE_TYPING` | `bigint` |
| `GUILD_PRESENCES` | `bigint` |
| `GUILD_SCHEDULED_EVENTS` | `bigint` |
| `GUILD_VOICE_STATES` | `bigint` |
| `GUILD_WEBHOOKS` | `bigint` |
| `MESSAGE_CONTENT` | `bigint` |

#### Defined in

src/classes/bitfields/Intents.ts:31

## Methods

### add

▸ **add**(...`flags`): [`Intents`](Intents.md)

Adds bits to the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``\>[] | The `BitResolvable`(s) to add. |

#### Returns

[`Intents`](Intents.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[add](Bitfield.md#add)

#### Defined in

src/classes/bitfields/Bitfield.ts:79

___

### clone

▸ **clone**(): [`Intents`](Intents.md)

Clones the Bitfield.

#### Returns

[`Intents`](Intents.md)

The cloned Bitfield.

#### Overrides

[Bitfield](Bitfield.md).[clone](Bitfield.md#clone)

#### Defined in

src/classes/bitfields/Intents.ts:42

___

### convert

▸ **convert**(`flags`): `bigint`

Converts a BitResolvable to a bigint.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flags` | [`BitResolvable`](modules.md#bitresolvable)<``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``\> \| [`BitResolvable`](modules.md#bitresolvable)<``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``\>[] | The `BitResolvable`(s) to convert. |

#### Returns

`bigint`

The bigint representation of the `BitResolvable`(s).

#### Inherited from

[Bitfield](Bitfield.md).[convert](Bitfield.md#convert)

#### Defined in

src/classes/bitfields/Bitfield.ts:43

___

### has

▸ **has**(...`flags`): `boolean`

Checks if the Bitfield has the given flag.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``\>[] | The `BitResolvable`(s) to check. |

#### Returns

`boolean`

Whether the Bitfield has the given flag(s).

#### Inherited from

[Bitfield](Bitfield.md).[has](Bitfield.md#has)

#### Defined in

src/classes/bitfields/Bitfield.ts:127

___

### isEmpty

▸ **isEmpty**(): `boolean`

Checks if the Bitfield is empty.

#### Returns

`boolean`

Whether the Bitfield is empty.

#### Inherited from

[Bitfield](Bitfield.md).[isEmpty](Bitfield.md#isempty)

#### Defined in

src/classes/bitfields/Bitfield.ts:136

___

### isLocked

▸ **isLocked**(): `boolean`

Check if the Bitfield is locked.

#### Returns

`boolean`

#### Inherited from

[Bitfield](Bitfield.md).[isLocked](Bitfield.md#islocked)

#### Defined in

src/classes/bitfields/Bitfield.ts:178

___

### remove

▸ **remove**(...`flags`): [`Intents`](Intents.md)

Removes bits from the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``\>[] | The `BitResolvable`(s) to remove. |

#### Returns

[`Intents`](Intents.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[remove](Bitfield.md#remove)

#### Defined in

src/classes/bitfields/Bitfield.ts:111

___

### set

▸ **set**(...`flags`): [`Intents`](Intents.md)

Sets the contents of the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``\>[] | The `BitResolvable`(s) to set. |

#### Returns

[`Intents`](Intents.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[set](Bitfield.md#set)

#### Defined in

src/classes/bitfields/Bitfield.ts:95

___

### toArray

▸ **toArray**(): (``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``)[]

Converts the Bitfield to an array of strings.

#### Returns

(``"GUILDS"`` \| ``"GUILD_MEMBERS"`` \| ``"GUILD_BANS"`` \| ``"GUILD_EMOJIS_AND_STICKERS"`` \| ``"GUILD_INTEGRATIONS"`` \| ``"GUILD_WEBHOOKS"`` \| ``"GUILD_INVITES"`` \| ``"GUILD_VOICE_STATES"`` \| ``"GUILD_PRESENCES"`` \| ``"GUILD_MESSAGES"`` \| ``"GUILD_MESSAGE_REACTIONS"`` \| ``"GUILD_MESSAGE_TYPING"`` \| ``"DIRECT_MESSAGES"`` \| ``"DIRECT_MESSAGE_REACTIONS"`` \| ``"DIRECT_MESSAGE_TYPING"`` \| ``"MESSAGE_CONTENT"`` \| ``"GUILD_SCHEDULED_EVENTS"`` \| ``"AUTO_MODERATION_CONFIGURATION"`` \| ``"AUTO_MODERATION_EXECUTION"``)[]

The array of strings representation of the Bitfield.

#### Inherited from

[Bitfield](Bitfield.md).[toArray](Bitfield.md#toarray)

#### Defined in

src/classes/bitfields/Bitfield.ts:154

___

### toBigInt

▸ **toBigInt**(): `bigint`

Converts the Bitfield to a bigint.

#### Returns

`bigint`

The bigint representation of the Bitfield.

#### Inherited from

[Bitfield](Bitfield.md).[toBigInt](Bitfield.md#tobigint)

#### Defined in

src/classes/bitfields/Bitfield.ts:145
