---
layout: default
title: "BirbAPIError"
parent: "Classes"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / [Exports](modules.md) / BirbAPIError

# Class: BirbAPIError

## Hierarchy

- [`BirbError`](BirbError.md)

  ↳ **`BirbAPIError`**

## Table of contents

### Constructors

- [constructor](BirbAPIError.md#constructor)

### Properties

- [body](BirbAPIError.md#body)
- [cause](BirbAPIError.md#cause)
- [endpoint](BirbAPIError.md#endpoint)
- [headers](BirbAPIError.md#headers)
- [json](BirbAPIError.md#json)
- [message](BirbAPIError.md#message)
- [name](BirbAPIError.md#name)
- [package](BirbAPIError.md#package)
- [stack](BirbAPIError.md#stack)
- [status](BirbAPIError.md#status)
- [prepareStackTrace](BirbAPIError.md#preparestacktrace)
- [stackTraceLimit](BirbAPIError.md#stacktracelimit)

### Methods

- [captureStackTrace](BirbAPIError.md#capturestacktrace)

## Constructors

### constructor

• **new BirbAPIError**(`message`, `request`, `status`, `json?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `request` | [`APIEndpoint`](APIEndpoint.md)<`any`, `any`, `any`\> |
| `status` | `number` |
| `json?` | `any` |

#### Overrides

[BirbError](BirbError.md).[constructor](BirbError.md#constructor)

#### Defined in

src/classes/errors/BirbAPIError.ts:11

## Properties

### body

• `Readonly` **body**: `any`

#### Defined in

src/classes/errors/BirbAPIError.ts:8

___

### cause

• `Optional` **cause**: `unknown`

#### Inherited from

[BirbError](BirbError.md).[cause](BirbError.md#cause)

#### Defined in

node_modules/typescript/lib/lib.es2022.error.d.ts:26

___

### endpoint

• `Readonly` **endpoint**: `string`

#### Defined in

src/classes/errors/BirbAPIError.ts:6

___

### headers

• `Readonly` **headers**: `Object`

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

src/classes/errors/BirbAPIError.ts:7

___

### json

• `Readonly` **json**: `any`

#### Defined in

src/classes/errors/BirbAPIError.ts:9

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

### status

• `Readonly` **status**: `number`

#### Defined in

src/classes/errors/BirbAPIError.ts:5

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
