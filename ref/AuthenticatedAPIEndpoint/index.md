---
layout: default
title: "AuthenticatedAPIEndpoint"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / AuthenticatedAPIEndpoint

# Class: AuthenticatedAPIEndpoint<Params, Response, Body\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `Params` | `Params` |
| `Response` | `Response` |
| `Body` | `any` |

## Hierarchy

- [`APIEndpoint`](../APIEndpoint/index.md)<`Params`, `Response`, `Body`\>

  ↳ **`AuthenticatedAPIEndpoint`**

  ↳↳ [`GetGuildRequest`](../GetGuildRequest/index.md)

  ↳↳ [`ModifyGuildRequest`](../ModifyGuildRequest/index.md)

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
- [furnishRequest](index.md#furnishrequest)
- [setAuditLogReason](index.md#setauditlogreason)
- [setBody](index.md#setbody)
- [setHeaders](index.md#setheaders)
- [setParams](index.md#setparams)
- [throwJSONError](index.md#throwjsonerror)

## Constructors

### constructor

• **new AuthenticatedAPIEndpoint**<`Params`, `Response`, `Body`\>(`client`, `method`)

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

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[constructor](../APIEndpoint/index.md#constructor)

#### Defined in

src/classes/api/APIEndpoint.ts:31

## Properties

### body

• **body**: `undefined` \| `Body`

The request body.

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[body](../APIEndpoint/index.md#body)

#### Defined in

src/classes/api/APIEndpoint.ts:29

___

### client

• **client**: [`Birb`](../Birb/index.md)

The Birb client.

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[client](../APIEndpoint/index.md#client)

#### Defined in

src/classes/api/APIEndpoint.ts:10

___

### headers

• **headers**: `Object`

The parameters to use.

#### Index signature

▪ [key: `string`]: `string`

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[headers](../APIEndpoint/index.md#headers)

#### Defined in

src/classes/api/APIEndpoint.ts:22

___

### method

• `Readonly` **method**: `string`

The method for the endpoint.

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[method](../APIEndpoint/index.md#method)

#### Defined in

src/classes/api/APIEndpoint.ts:14

___

### params

• **params**: `undefined` \| `Params`

The parameters to use.

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[params](../APIEndpoint/index.md#params)

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

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[buildURL](../APIEndpoint/index.md#buildurl)

#### Defined in

src/classes/api/APIEndpoint.ts:122

___

### execute

▸ **execute**(): `Promise`<[`APIResponse`](../modules.md#apiresponse)<`Response`\>\>

#### Returns

`Promise`<[`APIResponse`](../modules.md#apiresponse)<`Response`\>\>

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[execute](../APIEndpoint/index.md#execute)

#### Defined in

src/classes/api/APIEndpoint.ts:51

___

### furnishRequest

▸ `Protected` **furnishRequest**(): [`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Returns

[`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Overrides

APIEndpoint.furnishRequest

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:9

___

### setAuditLogReason

▸ **setAuditLogReason**(`reason?`): [`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `string` |

#### Returns

[`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:20

___

### setBody

▸ **setBody**(`body`): [`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `undefined` \| `Body` |

#### Returns

[`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[setBody](../APIEndpoint/index.md#setbody)

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[setHeaders](../APIEndpoint/index.md#setheaders)

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `Params` |

#### Returns

[`AuthenticatedAPIEndpoint`](index.md)<`Params`, `Response`, `Body`\>

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[setParams](../APIEndpoint/index.md#setparams)

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

#### Inherited from

[APIEndpoint](../APIEndpoint/index.md).[throwJSONError](../APIEndpoint/index.md#throwjsonerror)

#### Defined in

src/classes/api/APIEndpoint.ts:124
