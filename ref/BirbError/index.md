---
layout: default
title: "BirbError"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / BirbError

# Class: BirbError

## Hierarchy

- `Error`

  ↳ **`BirbError`**

  ↳↳ [`BirbAPIError`](../BirbAPIError/index.md)

  ↳↳ [`BirbGatewayDisconnection`](../BirbGatewayDisconnection/index.md)

  ↳↳ [`BirbValidationFailedError`](../BirbValidationFailedError/index.md)

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

• **new BirbError**(`message`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Overrides

Error.constructor

#### Defined in

src/classes/errors/BirbError.ts:4

## Properties

### cause

• `Optional` **cause**: `unknown`

#### Inherited from

Error.cause

#### Defined in

node_modules/typescript/lib/lib.es2022.error.d.ts:26

___

### message

• **message**: `string`

#### Inherited from

Error.message

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1041

___

### name

• **name**: `string`

#### Inherited from

Error.name

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1040

___

### package

• `Readonly` **package**: ``"birb"``

#### Defined in

src/classes/errors/BirbError.ts:2

___

### stack

• `Optional` **stack**: `string`

#### Inherited from

Error.stack

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1042

___

### prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

▸ (`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name | Type |
| :------ | :------ |
| `err` | `Error` |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

Error.prepareStackTrace

#### Defined in

node_modules/@types/node/globals.d.ts:11

___

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

Error.stackTraceLimit

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
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

Error.captureStackTrace

#### Defined in

node_modules/@types/node/globals.d.ts:4