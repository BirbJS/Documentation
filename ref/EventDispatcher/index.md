---
layout: default
title: "EventDispatcher"
parent: "1"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / EventDispatcher

# Class: EventDispatcher<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

## Hierarchy

- **`EventDispatcher`**

  ↳ [`Birb`](../Birb/index.md)

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Methods

- [clear](index.md#clear)
- [when](index.md#when)

## Constructors

### constructor

• **new EventDispatcher**<`T`\>()

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Defined in

src/classes/EventDispatcher.ts:10

## Methods

### clear

▸ **clear**(): `void`

#### Returns

`void`

#### Defined in

src/classes/EventDispatcher.ts:35

___

### when

▸ **when**(`event`): [`EventListener`](../EventListener/index.md)<`T`, [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function )\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `T` |

#### Returns

[`EventListener`](../EventListener/index.md)<`T`, [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function )\>

#### Defined in

src/classes/EventDispatcher.ts:14
