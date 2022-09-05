---
layout: default
title: "EventDispatcher"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / EventDispatcher

# Class: EventDispatcher<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

## Hierarchy

- **`EventDispatcher`**

  ↳ [`Birb`](Birb.md)

## Table of contents

### Constructors

- [constructor](EventDispatcher.md#constructor)

### Methods

- [clear](EventDispatcher.md#clear)
- [when](EventDispatcher.md#when)

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

▸ **when**(`event`): [`EventListener`](EventListener.md)<`T`, [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function )\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `T` |

#### Returns

[`EventListener`](EventListener.md)<`T`, [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function )\>

#### Defined in

src/classes/EventDispatcher.ts:14
