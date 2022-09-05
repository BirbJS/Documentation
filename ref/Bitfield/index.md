---
layout: default
title: "Bitfield"
parent: "1"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / Bitfield

# Class: Bitfield<K\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends `string` |

## Hierarchy

- **`Bitfield`**

  ↳ [`Intents`](../Intents/index.md)

  ↳ [`SystemChannelFlags`](../SystemChannelFlags/index.md)

  ↳ [`UserFlags`](../UserFlags/index.md)

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [bits](index.md#bits)

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

• **new Bitfield**<`K`\>(`bits`, `flags?`)

A Bitfield stores bits as bigints.

**`Params`**

flags The flags available to the Bitfield.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bits` | `number` \| `bigint` | The bigint or number representation of the Bitfield. |
| `flags?` | `Object` | - |

#### Defined in

src/classes/bitfields/Bitfield.ts:30

## Properties

### bits

• **bits**: `bigint`

The bits as a bigint.

#### Defined in

src/classes/bitfields/Bitfield.ts:10

## Methods

### add

▸ **add**(...`flags`): [`Bitfield`](index.md)<`K`\>

Adds bits to the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<`K`\>[] | The `BitResolvable`(s) to add. |

#### Returns

[`Bitfield`](index.md)<`K`\>

The updated Bitfield instance.

#### Defined in

src/classes/bitfields/Bitfield.ts:79

___

### clone

▸ `Abstract` **clone**(): [`Bitfield`](index.md)<`K`\>

Clones the Bitfield.

#### Returns

[`Bitfield`](index.md)<`K`\>

The cloned Bitfield.

#### Defined in

src/classes/bitfields/Bitfield.ts:22

___

### convert

▸ **convert**(`flags`): `bigint`

Converts a BitResolvable to a bigint.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flags` | [`BitResolvable`](../modules.md#bitresolvable)<`K`\> \| [`BitResolvable`](../modules.md#bitresolvable)<`K`\>[] | The `BitResolvable`(s) to convert. |

#### Returns

`bigint`

The bigint representation of the `BitResolvable`(s).

#### Defined in

src/classes/bitfields/Bitfield.ts:43

___

### has

▸ **has**(...`flags`): `boolean`

Checks if the Bitfield has the given flag.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<`K`\>[] | The `BitResolvable`(s) to check. |

#### Returns

`boolean`

Whether the Bitfield has the given flag(s).

#### Defined in

src/classes/bitfields/Bitfield.ts:127

___

### isEmpty

▸ **isEmpty**(): `boolean`

Checks if the Bitfield is empty.

#### Returns

`boolean`

Whether the Bitfield is empty.

#### Defined in

src/classes/bitfields/Bitfield.ts:136

___

### isLocked

▸ **isLocked**(): `boolean`

Check if the Bitfield is locked.

#### Returns

`boolean`

#### Defined in

src/classes/bitfields/Bitfield.ts:178

___

### remove

▸ **remove**(...`flags`): [`Bitfield`](index.md)<`K`\>

Removes bits from the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<`K`\>[] | The `BitResolvable`(s) to remove. |

#### Returns

[`Bitfield`](index.md)<`K`\>

The updated Bitfield instance.

#### Defined in

src/classes/bitfields/Bitfield.ts:111

___

### set

▸ **set**(...`flags`): [`Bitfield`](index.md)<`K`\>

Sets the contents of the Bitfield.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...flags` | [`BitResolvable`](../modules.md#bitresolvable)<`K`\>[] | The `BitResolvable`(s) to set. |

#### Returns

[`Bitfield`](index.md)<`K`\>

The updated Bitfield instance.

#### Defined in

src/classes/bitfields/Bitfield.ts:95

___

### toArray

▸ **toArray**(): `K`[]

Converts the Bitfield to an array of strings.

#### Returns

`K`[]

The array of strings representation of the Bitfield.

#### Defined in

src/classes/bitfields/Bitfield.ts:154

___

### toBigInt

▸ **toBigInt**(): `bigint`

Converts the Bitfield to a bigint.

#### Returns

`bigint`

The bigint representation of the Bitfield.

#### Defined in

src/classes/bitfields/Bitfield.ts:145
