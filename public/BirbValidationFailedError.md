---
layout: default
title: "BirbValidationFailedError"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / BirbValidationFailedError

# Class: BirbValidationFailedError

## Hierarchy

- [`BirbError`](BirbError.md)

  ↳ **`BirbValidationFailedError`**

## Table of contents

### Constructors

- [constructor](BirbValidationFailedError.md#constructor)

### Properties

- [cause](BirbValidationFailedError.md#cause)
- [data](BirbValidationFailedError.md#data)
- [message](BirbValidationFailedError.md#message)
- [name](BirbValidationFailedError.md#name)
- [package](BirbValidationFailedError.md#package)
- [stack](BirbValidationFailedError.md#stack)
- [prepareStackTrace](BirbValidationFailedError.md#preparestacktrace)
- [stackTraceLimit](BirbValidationFailedError.md#stacktracelimit)

### Methods

- [captureStackTrace](BirbValidationFailedError.md#capturestacktrace)

## Constructors

### constructor

• **new BirbValidationFailedError**(`message`, `data?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `data?` | `any` |

#### Overrides

[BirbError](BirbError.md).[constructor](BirbError.md#constructor)

#### Defined in

src/classes/errors/BirbValidationFailedError.ts:6

## Properties

### cause

• `Optional` **cause**: `unknown`

#### Inherited from

[BirbError](BirbError.md).[cause](BirbError.md#cause)

#### Defined in

node_modules/typescript/lib/lib.es2022.error.d.ts:26

___

### data

• `Readonly` **data**: `any`

#### Defined in

src/classes/errors/BirbValidationFailedError.ts:4

___

### message

• **message**: `string`

#### Inherited from

[BirbError](BirbError.md).[message](BirbError.md#message)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1041

___

### name

• **name**: `string`

#### Inherited from

[BirbError](BirbError.md).[name](BirbError.md#name)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1040

___

### package

• `Readonly` **package**: ``"birb"``

#### Inherited from

[BirbError](BirbError.md).[package](BirbError.md#package)

#### Defined in

src/classes/errors/BirbError.ts:2

___

### stack

• `Optional` **stack**: `string`

#### Inherited from

[BirbError](BirbError.md).[stack](BirbError.md#stack)

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

[BirbError](BirbError.md).[prepareStackTrace](BirbError.md#preparestacktrace)

#### Defined in

node_modules/@types/node/globals.d.ts:11

___

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

[BirbError](BirbError.md).[stackTraceLimit](BirbError.md#stacktracelimit)

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

[BirbError](BirbError.md).[captureStackTrace](BirbError.md#capturestacktrace)

#### Defined in

node_modules/@types/node/globals.d.ts:4
