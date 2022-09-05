---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / APIEndpoint

# Class: APIEndpoint<Params, Response, Body\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `Params` | `Params` |
| `Response` | `Response` |
| `Body` | `any` |

## Hierarchy

- **`APIEndpoint`**

  ↳ [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)

## Table of contents

### Constructors

- [constructor](APIEndpoint.md#constructor)

### Properties

- [body](APIEndpoint.md#body)
- [client](APIEndpoint.md#client)
- [headers](APIEndpoint.md#headers)
- [method](APIEndpoint.md#method)
- [params](APIEndpoint.md#params)

### Methods

- [buildURL](APIEndpoint.md#buildurl)
- [execute](APIEndpoint.md#execute)
- [setBody](APIEndpoint.md#setbody)
- [setHeaders](APIEndpoint.md#setheaders)
- [setParams](APIEndpoint.md#setparams)
- [throwJSONError](APIEndpoint.md#throwjsonerror)

## Constructors

### constructor

• **new APIEndpoint**<`Params`, `Response`, `Body`\>(`client`, `method`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `Params` | `Params` |
| `Response` | `Response` |
| `Body` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `method` | `string` |

#### Defined in

src/classes/api/APIEndpoint.ts:31

## Properties

### body

• **body**: `undefined` \| `Body`

The request body.

#### Defined in

src/classes/api/APIEndpoint.ts:29

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Defined in

src/classes/api/APIEndpoint.ts:10

___

### headers

• **headers**: `Object`

The parameters to use.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

src/classes/api/APIEndpoint.ts:22

___

### method

• `Readonly` **method**: `string`

The method for the endpoint.

#### Defined in

src/classes/api/APIEndpoint.ts:14

___

### params

• **params**: `undefined` \| `Params`

The parameters to use.

#### Defined in

src/classes/api/APIEndpoint.ts:18

## Methods

### buildURL

▸ `Abstract` **buildURL**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `Params` |

#### Returns

`string`

#### Defined in

src/classes/api/APIEndpoint.ts:122

___

### execute

▸ **execute**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](modules.md#apiresponse)<`Response`\>\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](modules.md#apiresponse)<`Response`\>\>

#### Defined in

src/classes/api/APIEndpoint.ts:51

___

### setBody

▸ **setBody**(`body`): [`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `undefined` \| `Body` |

#### Returns

[`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `Params` |

#### Returns

[`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/APIEndpoint.ts:41

___

### throwJSONError

▸ **throwJSONError**(`response`, `json?`): [`BirbAPIError`](BirbAPIError.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `Response` |
| `json?` | `any` |

#### Returns

[`BirbAPIError`](BirbAPIError.md)

#### Defined in

src/classes/api/APIEndpoint.ts:124
