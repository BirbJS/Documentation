---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / AuthenticatedAPIEndpoint

# Class: AuthenticatedAPIEndpoint<Params, Response, Body\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `Params` | `Params` |
| `Response` | `Response` |
| `Body` | `any` |

## Hierarchy

- [`APIEndpoint`](APIEndpoint.md)<`Params`, `Response`, `Body`\>

  ↳ **`AuthenticatedAPIEndpoint`**

  ↳↳ [`GetGuildRequest`](GetGuildRequest.md)

  ↳↳ [`ModifyGuildRequest`](ModifyGuildRequest.md)

## Table of contents

### Constructors

- [constructor](AuthenticatedAPIEndpoint.md#constructor)

### Properties

- [body](AuthenticatedAPIEndpoint.md#body)
- [client](AuthenticatedAPIEndpoint.md#client)
- [headers](AuthenticatedAPIEndpoint.md#headers)
- [method](AuthenticatedAPIEndpoint.md#method)
- [params](AuthenticatedAPIEndpoint.md#params)

### Methods

- [buildURL](AuthenticatedAPIEndpoint.md#buildurl)
- [execute](AuthenticatedAPIEndpoint.md#execute)
- [furnishRequest](AuthenticatedAPIEndpoint.md#furnishrequest)
- [setAuditLogReason](AuthenticatedAPIEndpoint.md#setauditlogreason)
- [setBody](AuthenticatedAPIEndpoint.md#setbody)
- [setHeaders](AuthenticatedAPIEndpoint.md#setheaders)
- [setParams](AuthenticatedAPIEndpoint.md#setparams)
- [throwJSONError](AuthenticatedAPIEndpoint.md#throwjsonerror)

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
| `client` | [`Birb`](Birb.md) |
| `method` | `string` |

#### Inherited from

[APIEndpoint](APIEndpoint.md).[constructor](APIEndpoint.md#constructor)

#### Defined in

src/classes/api/APIEndpoint.ts:31

## Properties

### body

• **body**: `undefined` \| `Body`

The request body.

#### Inherited from

[APIEndpoint](APIEndpoint.md).[body](APIEndpoint.md#body)

#### Defined in

src/classes/api/APIEndpoint.ts:29

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Inherited from

[APIEndpoint](APIEndpoint.md).[client](APIEndpoint.md#client)

#### Defined in

src/classes/api/APIEndpoint.ts:10

___

### headers

• **headers**: `Object`

The parameters to use.

#### Index signature

▪ [key: `string`]: `string`

#### Inherited from

[APIEndpoint](APIEndpoint.md).[headers](APIEndpoint.md#headers)

#### Defined in

src/classes/api/APIEndpoint.ts:22

___

### method

• `Readonly` **method**: `string`

The method for the endpoint.

#### Inherited from

[APIEndpoint](APIEndpoint.md).[method](APIEndpoint.md#method)

#### Defined in

src/classes/api/APIEndpoint.ts:14

___

### params

• **params**: `undefined` \| `Params`

The parameters to use.

#### Inherited from

[APIEndpoint](APIEndpoint.md).[params](APIEndpoint.md#params)

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

[APIEndpoint](APIEndpoint.md).[buildURL](APIEndpoint.md#buildurl)

#### Defined in

src/classes/api/APIEndpoint.ts:122

___

### execute

▸ **execute**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](modules.md#apiresponse)<`Response`\>\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](modules.md#apiresponse)<`Response`\>\>

#### Inherited from

[APIEndpoint](APIEndpoint.md).[execute](APIEndpoint.md#execute)

#### Defined in

src/classes/api/APIEndpoint.ts:51

___

### furnishRequest

▸ `Protected` **furnishRequest**(): [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Returns

[`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Overrides

APIEndpoint.furnishRequest

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:9

___

### setAuditLogReason

▸ **setAuditLogReason**(`reason?`): [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `string` |

#### Returns

[`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:20

___

### setBody

▸ **setBody**(`body`): [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `undefined` \| `Body` |

#### Returns

[`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Inherited from

[APIEndpoint](APIEndpoint.md).[setBody](APIEndpoint.md#setbody)

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Inherited from

[APIEndpoint](APIEndpoint.md).[setHeaders](APIEndpoint.md#setheaders)

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `Params` |

#### Returns

[`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<`Params`, `Response`, `Body`\>

#### Inherited from

[APIEndpoint](APIEndpoint.md).[setParams](APIEndpoint.md#setparams)

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

#### Inherited from

[APIEndpoint](APIEndpoint.md).[throwJSONError](APIEndpoint.md#throwjsonerror)

#### Defined in

src/classes/api/APIEndpoint.ts:124
