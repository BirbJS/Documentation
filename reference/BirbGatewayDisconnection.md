---
layout: default
title: BirbGatewayDisconnection
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / BirbGatewayDisconnection

# Class: BirbGatewayDisconnection

## Hierarchy

- [`BirbError`](BirbError.md)

  ↳ **`BirbGatewayDisconnection`**

## Table of contents

### Constructors

- [constructor](BirbGatewayDisconnection.md#constructor)

### Properties

- [cause](BirbGatewayDisconnection.md#cause)
- [message](BirbGatewayDisconnection.md#message)
- [name](BirbGatewayDisconnection.md#name)
- [package](BirbGatewayDisconnection.md#package)
- [stack](BirbGatewayDisconnection.md#stack)
- [prepareStackTrace](BirbGatewayDisconnection.md#preparestacktrace)
- [stackTraceLimit](BirbGatewayDisconnection.md#stacktracelimit)

### Methods

- [captureStackTrace](BirbGatewayDisconnection.md#capturestacktrace)

## Constructors

### constructor

• **new BirbGatewayDisconnection**(`message`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Overrides

[BirbError](BirbError.md).[constructor](BirbError.md#constructor)

#### Defined in

src/classes/errors/BirbGatewayDisconnection.ts:4

## Properties

### cause

• `Optional` **cause**: `unknown`

#### Inherited from

[BirbError](BirbError.md).[cause](BirbError.md#cause)

#### Defined in

node_modules/typescript/lib/lib.es2022.error.d.ts:26

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
