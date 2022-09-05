---
layout: default
title: "SystemChannelFlags"
parent: "1"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / SystemChannelFlags

# Class: SystemChannelFlags

## Hierarchy

- [`Bitfield`](../Bitfield/index.md)<[`SystemChannelFlagsString`](../modules.md#systemchannelflagsstring)\>

  ↳ **`SystemChannelFlags`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [bits](index.md#bits)
- [FLAGS](index.md#flags)

### Methods

- [add](index.md#add)
- [clone](index.md#clone)
- [convert](index.md#convert)
- [has](index.md#has)
- [isEmpty](index.md#isempty)
- [isLocked](index.md#islocked)
- [remove](index.md#remove)
- [set](index.md#set)
- [toArray](index.md#toarray)
- [toBigInt](index.md#tobigint)

## Constructors

### constructor

• **new SystemChannelFlags**(`bits?`)

The Intents Bitfield stores bits as bigints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bits?` | `number` \| `bigint` | The bigint or number representation of the Bitfield. |

#### Overrides

[Bitfield](../Bitfield/index.md).[constructor](../Bitfield/index.md#constructor)

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:24

## Properties

### bits

• **bits**: `bigint`

The bits as a bigint.

#### Inherited from

[Bitfield](../Bitfield/index.md).[bits](../Bitfield/index.md#bits)

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

▸ **add**(...`flags`): [`SystemChannelFlags`](index.md)

Adds bits to the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to add. |

#### Returns

[`SystemChannelFlags`](index.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](../Bitfield/index.md).[add](../Bitfield/index.md#add)

#### Defined in

src/classes/bitfields/Bitfield.ts:79

___

### clone

▸ **clone**(): [`SystemChannelFlags`](index.md)

Clones the Bitfield.

#### Returns

[`SystemChannelFlags`](index.md)

The cloned Bitfield.

#### Overrides

[Bitfield](../Bitfield/index.md).[clone](../Bitfield/index.md#clone)

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:28

___

### convert

▸ **convert**(`flags`): `bigint`

Converts a BitResolvable to a bigint.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flags` | [`BitResolvable`](../modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\> \| [`BitResolvable`](../modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to convert. |

#### Returns

`bigint`

The bigint representation of the `BitResolvable`(s).

#### Inherited from

[Bitfield](../Bitfield/index.md).[convert](../Bitfield/index.md#convert)

#### Defined in

src/classes/bitfields/Bitfield.ts:43

___

### has

▸ **has**(...`flags`): `boolean`

Checks if the Bitfield has the given flag.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to check. |

#### Returns

`boolean`

Whether the Bitfield has the given flag(s).

#### Inherited from

[Bitfield](../Bitfield/index.md).[has](../Bitfield/index.md#has)

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

[Bitfield](../Bitfield/index.md).[isEmpty](../Bitfield/index.md#isempty)

#### Defined in

src/classes/bitfields/Bitfield.ts:136

___

### isLocked

▸ **isLocked**(): `boolean`

Check if the Bitfield is locked.

#### Returns

`boolean`

#### Inherited from

[Bitfield](../Bitfield/index.md).[isLocked](../Bitfield/index.md#islocked)

#### Defined in

src/classes/bitfields/Bitfield.ts:178

___

### remove

▸ **remove**(...`flags`): [`SystemChannelFlags`](index.md)

Removes bits from the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to remove. |

#### Returns

[`SystemChannelFlags`](index.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](../Bitfield/index.md).[remove](../Bitfield/index.md#remove)

#### Defined in

src/classes/bitfields/Bitfield.ts:111

___

### set

▸ **set**(...`flags`): [`SystemChannelFlags`](index.md)

Sets the contents of the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<``"SUPPRESS_JOIN_NOTIFICATIONS"`` \| ``"SUPPRESS_PREMIUM_SUBSCRIPTIONS"`` \| ``"SUPPRESS_GUILD_REMINDER_NOTIFICATIONS"`` \| ``"SUPPRESS_JOIN_NOTIFICATION_REPLIES"``\>[] | The `BitResolvable`(s) to set. |

#### Returns

[`SystemChannelFlags`](index.md)

The updated Bitfield instance.

#### Inherited from

[Bitfield](../Bitfield/index.md).[set](../Bitfield/index.md#set)

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

[Bitfield](../Bitfield/index.md).[toArray](../Bitfield/index.md#toarray)

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

[Bitfield](../Bitfield/index.md).[toBigInt](../Bitfield/index.md#tobigint)

#### Defined in

src/classes/bitfields/Bitfield.ts:145
