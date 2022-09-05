---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / SystemChannelFlags

# Class: SystemChannelFlags

## Hierarchy

- [`Bitfield`](Bitfield.md)<[`SystemChannelFlagsString`](modules.md#systemchannelflagsstring)\>

  ↳ **`SystemChannelFlags`**

## Table of contents

### Constructors

- [constructor](SystemChannelFlags.md#constructor)

### Properties

- [bits](SystemChannelFlags.md#bits)
- [FLAGS](SystemChannelFlags.md#flags)

### Methods

- [add](SystemChannelFlags.md#add)
- [clone](SystemChannelFlags.md#clone)
- [convert](SystemChannelFlags.md#convert)
- [has](SystemChannelFlags.md#has)
- [isEmpty](SystemChannelFlags.md#isempty)
- [isLocked](SystemChannelFlags.md#islocked)
- [remove](SystemChannelFlags.md#remove)
- [set](SystemChannelFlags.md#set)
- [toArray](SystemChannelFlags.md#toarray)
- [toBigInt](SystemChannelFlags.md#tobigint)

## Constructors

### constructor

• **new SystemChannelFlags**(`bits?`)

The Intents Bitfield stores bits as bigints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bits?` | `number` \| `bigint` | The bigint or number representation of the Bitfield. |

#### Overrides

[Bitfield](Bitfield.md).[constructor](Bitfield.md#constructor)

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:24

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

▪ `Static` `Readonly` **FLAGS**: `Object` = `SystemChannelFlag`

The possible Intents the client can use.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `SUPPRESS_GUILD_REMINDER_NOTIFICATIONS` | `bigint` |
| `SUPPRESS_JOIN_NOTIFICATIONS` | `bigint` |
| `SUPPRESS_JOIN_NOTIFICATION_REPLIES` | `bigint` |
| `SUPPRESS_PREMIUM_SUBSCRIPTIONS` | `bigint` |

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:17

## Methods

### add

▸ **add**(...`flags`): [`SystemChannelFlags`](SystemChannelFlags.md)

Adds bits to the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to add. |

#### Returns

[`SystemChannelFlags`](SystemChannelFlags.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[add](Bitfield.md#add)

#### Defined in

src/classes/bitfields/Bitfield.ts:79

___

### clone

▸ **clone**(): [`SystemChannelFlags`](SystemChannelFlags.md)

Clones the Bitfield.

#### Returns

[`SystemChannelFlags`](SystemChannelFlags.md)

The cloned Bitfield.

#### Overrides

[Bitfield](Bitfield.md).[clone](Bitfield.md#clone)

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:28

___

### convert

▸ **convert**(`flags`): `bigint`

Converts a BitResolvable to a bigint.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flags` | [`BitResolvable`](modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\> \| [`BitResolvable`](modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to convert. |

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
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to check. |

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

▸ **remove**(...`flags`): [`SystemChannelFlags`](SystemChannelFlags.md)

Removes bits from the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to remove. |

#### Returns

[`SystemChannelFlags`](SystemChannelFlags.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[remove](Bitfield.md#remove)

#### Defined in

src/classes/bitfields/Bitfield.ts:111

___

### set

▸ **set**(...`flags`): [`SystemChannelFlags`](SystemChannelFlags.md)

Sets the contents of the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to set. |

#### Returns

[`SystemChannelFlags`](SystemChannelFlags.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](Bitfield.md).[set](Bitfield.md#set)

#### Defined in

src/classes/bitfields/Bitfield.ts:95

___

### toArray

▸ **toArray**(): (``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``)[]

Converts the Bitfield to an array of strings.

#### Returns

(``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``)[]

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
