---
layout: default
title: EventListener
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / EventListener

# Class: EventListener<E, F\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `E` | extends `string` |
| `F` | extends [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function ) |

## Table of contents

### Constructors

- [constructor](EventListener.md#constructor)

### Methods

- [do](EventListener.md#do)
- [forget](EventListener.md#forget)
- [once](EventListener.md#once)

## Constructors

### constructor

• **new EventListener**<`E`, `F`\>(`parent`, `event`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `E` | extends `string` |
| `F` | extends [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function ) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `parent` | [`EventDispatcher`](EventDispatcher.md)<`E`\> |
| `event` | `E` |

#### Defined in

src/classes/EventListener.ts:10

## Methods

### do

▸ **do**(`handler`): [`EventListener`](EventListener.md)<`E`, `F`\>

Add a handler that should be called.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handler` | `F` | The function. |

#### Returns

[`EventListener`](EventListener.md)<`E`, `F`\>

The EventListener for chaining.

#### Defined in

src/classes/EventListener.ts:21

___

### forget

▸ **forget**(): `void`

Forgets the EventListener, removing it from the EventDispatcher. This
will result in the EventListener no longer being called when the parent
EventDispatcher is used to dispatch an event.

#### Returns

`void`

#### Defined in

src/classes/EventListener.ts:57

___

### once

▸ **once**(): [`EventListener`](EventListener.md)<`E`, `F`\>

Sets the EventListener to only dispatch once. When the EventListener is
dispatched, the `forget()` method is called internally.

#### Returns

[`EventListener`](EventListener.md)<`E`, `F`\>

The EventListener for chaining.

#### Defined in

src/classes/EventListener.ts:47
