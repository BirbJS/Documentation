---
layout: default
title: "APIEndpoint"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / APIEndpoint

# Class: APIEndpoint<Params, Response, Body\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `Params` | `Params` |
| `Response` | `Response` |
| `Body` | `any` |

## Hierarchy

- **`APIEndpoint`**

  ↳ [`AuthenticatedAPIEndpoint`](../AuthenticatedAPIEndpoint/index.md)

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [body](index.md#body)
- [client](index.md#client)
- [headers](index.md#headers)
- [method](index.md#method)
- [params](index.md#params)

### Methods

- [buildURL](index.md#buildurl)
- [execute](index.md#execute)
- [setBody](index.md#setbody)
- [setHeaders](index.md#setheaders)
- [setParams](index.md#setparams)
- [throwJSONError](index.md#throwjsonerror)

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
| `client` | [`Birb`](../Birb/index.md) |
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

• **client**: [`Birb`](../Birb/index.md)

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

▸ **execute**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](../modules.md#apiresponse)<`Response`\>\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](../modules.md#apiresponse)<`Response`\>\>

#### Defined in

src/classes/api/APIEndpoint.ts:51

___

### setBody

▸ **setBody**(`body`): [`APIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `undefined` \| `Body` |

#### Returns

[`APIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`APIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`APIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`APIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `Params` |

#### Returns

[`APIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/APIEndpoint.ts:41

___

### throwJSONError

▸ **throwJSONError**(`response`, `json?`): [`BirbAPIError`](../BirbAPIError/index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `Response` |
| `json?` | `any` |

#### Returns

[`BirbAPIError`](../BirbAPIError/index.md)

#### Defined in

src/classes/api/APIEndpoint.ts:124
