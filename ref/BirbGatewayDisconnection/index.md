---
layout: default
title: "BirbGatewayDisconnection"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / BirbGatewayDisconnection

# Class: BirbGatewayDisconnection

## Hierarchy

- [`BirbError`](../BirbError/index.md)

  ↳ **`BirbGatewayDisconnection`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [cause](index.md#cause)
- [message](index.md#message)
- [name](index.md#name)
- [package](index.md#package)
- [stack](index.md#stack)
- [prepareStackTrace](index.md#preparestacktrace)
- [stackTraceLimit](index.md#stacktracelimit)

### Methods

- [captureStackTrace](index.md#capturestacktrace)

## Constructors

### constructor

• **new BirbGatewayDisconnection**(`message`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Overrides

[BirbError](../BirbError/index.md).[constructor](../BirbError/index.md#constructor)

#### Defined in

src/classes/errors/BirbGatewayDisconnection.ts:4

## Properties

### cause

• `Optional` **cause**: `unknown`

#### Inherited from

[BirbError](../BirbError/index.md).[cause](../BirbError/index.md#cause)

#### Defined in

node_modules/typescript/lib/lib.es2022.error.d.ts:26

___

### message

• **message**: `string`

#### Inherited from

[BirbError](../BirbError/index.md).[message](../BirbError/index.md#message)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1041

___

### name

• **name**: `string`

#### Inherited from

[BirbError](../BirbError/index.md).[name](../BirbError/index.md#name)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1040

___

### package

• `Readonly` **package**: ``"birb"``

#### Inherited from

[BirbError](../BirbError/index.md).[package](../BirbError/index.md#package)

#### Defined in

src/classes/errors/BirbError.ts:2

___

### stack

• `Optional` **stack**: `string`

#### Inherited from

[BirbError](../BirbError/index.md).[stack](../BirbError/index.md#stack)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1042

___

### prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: [`Error`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error ), `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

▸ (`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name | Type |
| :------ | :------ |
| `err` | [`Error`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error ) |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

[BirbError](../BirbError/index.md).[prepareStackTrace](../BirbError/index.md#preparestacktrace)

#### Defined in

node_modules/@types/node/globals.d.ts:11

___

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

[BirbError](../BirbError/index.md).[stackTraceLimit](../BirbError/index.md#stacktracelimit)

#### Defined in

node_modules/@types/node/globals.d.ts:13

## Methods

### captureStackTrace

▸ `Static` **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetObject` | `object` |
| `constructorOpt?` | [`Function`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function ) |

#### Returns

`void`

#### Inherited from

[BirbError](../BirbError/index.md).[captureStackTrace](../BirbError/index.md#capturestacktrace)

#### Defined in

node_modules/@types/node/globals.d.ts:4
