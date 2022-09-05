---
layout: default
title: "Cache"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / Cache

# Class: Cache<K, T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `K` | `string` |
| `T` | `any` |

## Table of contents

### Constructors

- [constructor](Cache.md#constructor)

### Properties

- [client](Cache.md#client)

### Methods

- [entries](Cache.md#entries)
- [filter](Cache.md#filter)
- [find](Cache.md#find)
- [get](Cache.md#get)
- [has](Cache.md#has)
- [keys](Cache.md#keys)
- [remove](Cache.md#remove)
- [set](Cache.md#set)
- [size](Cache.md#size)
- [take](Cache.md#take)
- [toArray](Cache.md#toarray)
- [values](Cache.md#values)

## Constructors

### constructor

• **new Cache**<`K`, `T`\>(`client`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | `string` |
| `T` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |

#### Defined in

src/classes/Cache.ts:14

## Properties

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Defined in

src/classes/Cache.ts:8

## Methods

### entries

▸ **entries**(): `IterableIterator`<[`K`, `T`]\>

#### Returns

`IterableIterator`<[`K`, `T`]\>

#### Defined in

src/classes/Cache.ts:61

___

### filter

▸ **filter**(`fn`): [`Pair`](Pair.md)<`K`, `T`\>[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `fn` | (`e`: [`Pair`](Pair.md)<`K`, `T`\>) => `boolean` |

#### Returns

[`Pair`](Pair.md)<`K`, `T`\>[]

#### Defined in

src/classes/Cache.ts:27

___

### find

▸ **find**(`fn`): `undefined` \| [`Pair`](Pair.md)<`K`, `T`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `fn` | (`e`: [`Pair`](Pair.md)<`K`, `T`\>) => `boolean` |

#### Returns

`undefined` \| [`Pair`](Pair.md)<`K`, `T`\>

#### Defined in

src/classes/Cache.ts:23

___

### get

▸ **get**(`key`): `undefined` \| `T`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `K` |

#### Returns

`undefined` \| `T`

#### Defined in

src/classes/Cache.ts:19

___

### has

▸ **has**(`key`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `K` |

#### Returns

`boolean`

#### Defined in

src/classes/Cache.ts:35

___

### keys

▸ **keys**(): `IterableIterator`<`K`\>

#### Returns

`IterableIterator`<`K`\>

#### Defined in

src/classes/Cache.ts:53

___

### remove

▸ **remove**(`key`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `K` |

#### Returns

`void`

#### Defined in

src/classes/Cache.ts:39

___

### set

▸ **set**(`key`, `value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `K` |
| `value` | `T` |

#### Returns

`void`

#### Defined in

src/classes/Cache.ts:31

___

### size

▸ **size**(): `number`

#### Returns

`number`

#### Defined in

src/classes/Cache.ts:49

___

### take

▸ **take**(`key`): `undefined` \| `T`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `K` |

#### Returns

`undefined` \| `T`

#### Defined in

src/classes/Cache.ts:43

___

### toArray

▸ **toArray**(): [`Pair`](Pair.md)<`K`, `T`\>[]

#### Returns

[`Pair`](Pair.md)<`K`, `T`\>[]

#### Defined in

src/classes/Cache.ts:65

___

### values

▸ **values**(): `IterableIterator`<`T`\>

#### Returns

`IterableIterator`<`T`\>

#### Defined in

src/classes/Cache.ts:57
