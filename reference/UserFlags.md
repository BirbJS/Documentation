---
layout: default
title: UserFlags
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / UserFlags

# Class: UserFlags

## Hierarchy

- [`Bitfield`](Bitfield.md)<[`UserFlagsString`](modules.md#userflagsstring)\>

  ↳ **`UserFlags`**

## Table of contents

### Constructors

- [constructor](UserFlags.md#constructor)

### Properties

- [bits](UserFlags.md#bits)
- [FLAGS](UserFlags.md#flags)

### Methods

- [add](UserFlags.md#add)
- [clone](UserFlags.md#clone)
- [convert](UserFlags.md#convert)
- [has](UserFlags.md#has)
- [isEmpty](UserFlags.md#isempty)
- [isLocked](UserFlags.md#islocked)
- [remove](UserFlags.md#remove)
- [set](UserFlags.md#set)
- [toArray](UserFlags.md#toarray)
- [toBigInt](UserFlags.md#tobigint)

## Constructors

### constructor

• **new UserFlags**(`bits?`)

The Intents Bitfield stores bits as bigints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bits?` | `number` \| `bigint` | The bigint or number representation of the Bitfield. |

#### Overrides

[Bitfield](Bitfield.md).[constructor](Bitfield.md#constructor)

#### Defined in

src/classes/bitfields/UserFlags.ts:76

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

▪ `Static` `Readonly` **FLAGS**: `Object` = `UserFlag`

The possible Intents the client can use.

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `BOT_HTTP_INTERACTIONS` | `bigint` | A bot that uses only [HTTP interactions](https://discord.com/developers/docs/interactions/receiving-and-responding#receiving-an-interaction) and is shown in the online member list |
| `BUG_HUNTER_LEVEL_1` | `bigint` | Bug Hunter Level 1 |
| `BUG_HUNTER_LEVEL_2` | `bigint` | Bug Hunter Level 2 |
| `CERTIFIED_MODERATOR` | `bigint` | Discord Certified Moderator |
| `HYPESQUAD` | `bigint` | HypeSquad Events Member |
| `HYPESQUAD_ONLINE_HOUSE_BALANCE` | `bigint` | House Balance Member |
| `HYPESQUAD_ONLINE_HOUSE_BRAVERY` | `bigint` | House Bravery Member |
| `HYPESQUAD_ONLINE_HOUSE_BRILLIANCE` | `bigint` | House Brilliance Member |
| `NITRO_EARLY_SUPPORTER` | `bigint` | Early Nitro Supporter |
| `PARTNER` | `bigint` | Partnered Server Owner |
| `STAFF` | `bigint` | Discord Employee or Staff Member |
| `TEAM_PSEUDO_USER` | `bigint` | The user is actually a [team](https://discord.com/developers/docs/topics/teams) |
| `VERIFIED_BOT` | `bigint` | Verified Bot |
| `VERIFIED_BOT_DEVELOPER` | `bigint` | Early Verified Bot Developer |

#### Defined in

src/classes/bitfields/UserFlags.ts:69

## Methods

### add

▸ **add**(...`flags`): [`UserFlags`](UserFlags.md)

Adds bits to the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``\>[] | The `BitResolvable`(s) to add. |

#### Returns

[`UserFlags`](UserFlags.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[add](Bitfield.md#add)

#### Defined in

src/classes/bitfields/Bitfield.ts:79

___

### clone

▸ **clone**(): [`UserFlags`](UserFlags.md)

Clones the Bitfield.

#### Returns

[`UserFlags`](UserFlags.md)

The cloned Bitfield.

#### Overrides

[Bitfield](Bitfield.md).[clone](Bitfield.md#clone)

#### Defined in

src/classes/bitfields/UserFlags.ts:80

___

### convert

▸ **convert**(`flags`): `bigint`

Converts a BitResolvable to a bigint.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flags` | [`BitResolvable`](modules.md#bitresolvable)<``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``\> \| [`BitResolvable`](modules.md#bitresolvable)<``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``\>[] | The `BitResolvable`(s) to convert. |

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
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``\>[] | The `BitResolvable`(s) to check. |

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

▸ **remove**(...`flags`): [`UserFlags`](UserFlags.md)

Removes bits from the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``\>[] | The `BitResolvable`(s) to remove. |

#### Returns

[`UserFlags`](UserFlags.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[remove](Bitfield.md#remove)

#### Defined in

src/classes/bitfields/Bitfield.ts:111

___

### set

▸ **set**(...`flags`): [`UserFlags`](UserFlags.md)

Sets the contents of the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``\>[] | The `BitResolvable`(s) to set. |

#### Returns

[`UserFlags`](UserFlags.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[set](Bitfield.md#set)

#### Defined in

src/classes/bitfields/Bitfield.ts:95

___

### toArray

▸ **toArray**(): (``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``)[]

Converts the Bitfield to an array of strings.

#### Returns

(``"STAFF"`` \| ``"PARTNER"`` \| ``"HYPESQUAD"`` \| ``"BUG_HUNTER_LEVEL_1"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRAVERY"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BRILLIANCE"`` \| ``"HYPESQUAD_ONLINE_HOUSE_BALANCE"`` \| ``"NITRO_EARLY_SUPPORTER"`` \| ``"TEAM_PSEUDO_USER"`` \| ``"BUG_HUNTER_LEVEL_2"`` \| ``"VERIFIED_BOT"`` \| ``"VERIFIED_BOT_DEVELOPER"`` \| ``"CERTIFIED_MODERATOR"`` \| ``"BOT_HTTP_INTERACTIONS"``)[]

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
