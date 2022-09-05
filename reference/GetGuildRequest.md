---
layout: default
title: Modules
parent: Reference
has_toc: false
nav_order: 5
---

[Birb](/) / GetGuildRequest

# Class: GetGuildRequest

## Hierarchy

- [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<[`GetGuildParams`](modules.md#getguildparams), [`APIGuild`](modules.md#apiguild)\>

  ↳ **`GetGuildRequest`**

## Table of contents

### Constructors

- [constructor](GetGuildRequest.md#constructor)

### Properties

- [body](GetGuildRequest.md#body)
- [client](GetGuildRequest.md#client)
- [headers](GetGuildRequest.md#headers)
- [method](GetGuildRequest.md#method)
- [params](GetGuildRequest.md#params)

### Methods

- [buildURL](GetGuildRequest.md#buildurl)
- [execute](GetGuildRequest.md#execute)
- [furnishRequest](GetGuildRequest.md#furnishrequest)
- [setAuditLogReason](GetGuildRequest.md#setauditlogreason)
- [setBody](GetGuildRequest.md#setbody)
- [setHeaders](GetGuildRequest.md#setheaders)
- [setParams](GetGuildRequest.md#setparams)
- [throwJSONError](GetGuildRequest.md#throwjsonerror)
- [validateResponse](GetGuildRequest.md#validateresponse)

## Constructors

### constructor

• **new GetGuildRequest**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |

#### Overrides

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[constructor](AuthenticatedAPIEndpoint.md#constructor)

#### Defined in

src/classes/api/endpoints/GetGuildRequest.ts:16

## Properties

### body

• **body**: `any`

The request body.

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[body](AuthenticatedAPIEndpoint.md#body)

#### Defined in

src/classes/api/APIEndpoint.ts:29

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client.

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[client](AuthenticatedAPIEndpoint.md#client)

#### Defined in

src/classes/api/APIEndpoint.ts:10

___

### headers

• **headers**: `Object`

The parameters to use.

#### Index signature

▪ [key: `string`]: `string`

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[headers](AuthenticatedAPIEndpoint.md#headers)

#### Defined in

src/classes/api/APIEndpoint.ts:22

___

### method

• `Readonly` **method**: `string`

The method for the endpoint.

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[method](AuthenticatedAPIEndpoint.md#method)

#### Defined in

src/classes/api/APIEndpoint.ts:14

___

### params

• **params**: `undefined` \| [`GetGuildParams`](modules.md#getguildparams)

The parameters to use.

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[params](AuthenticatedAPIEndpoint.md#params)

#### Defined in

src/classes/api/APIEndpoint.ts:18

## Methods

### buildURL

▸ **buildURL**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`GetGuildParams`](modules.md#getguildparams) |

#### Returns

`string`

#### Overrides

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[buildURL](AuthenticatedAPIEndpoint.md#buildurl)

#### Defined in

src/classes/api/endpoints/GetGuildRequest.ts:20

___

### execute

▸ **execute**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](modules.md#apiresponse)<[`APIGuild`](modules.md#apiguild)\>\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`APIResponse`](modules.md#apiresponse)<[`APIGuild`](modules.md#apiguild)\>\>

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[execute](AuthenticatedAPIEndpoint.md#execute)

#### Defined in

src/classes/api/APIEndpoint.ts:51

___

### furnishRequest

▸ `Protected` **furnishRequest**(): [`GetGuildRequest`](GetGuildRequest.md)

#### Returns

[`GetGuildRequest`](GetGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[furnishRequest](AuthenticatedAPIEndpoint.md#furnishrequest)

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:9

___

### setAuditLogReason

▸ **setAuditLogReason**(`reason?`): [`GetGuildRequest`](GetGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `string` |

#### Returns

[`GetGuildRequest`](GetGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setAuditLogReason](AuthenticatedAPIEndpoint.md#setauditlogreason)

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:20

___

### setBody

▸ **setBody**(`body`): [`GetGuildRequest`](GetGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `any` |

#### Returns

[`GetGuildRequest`](GetGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setBody](AuthenticatedAPIEndpoint.md#setbody)

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`GetGuildRequest`](GetGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`GetGuildRequest`](GetGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setHeaders](AuthenticatedAPIEndpoint.md#setheaders)

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`GetGuildRequest`](GetGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`GetGuildParams`](modules.md#getguildparams) |

#### Returns

[`GetGuildRequest`](GetGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setParams](AuthenticatedAPIEndpoint.md#setparams)

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

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[throwJSONError](AuthenticatedAPIEndpoint.md#throwjsonerror)

#### Defined in

src/classes/api/APIEndpoint.ts:124

___

### validateResponse

▸ **validateResponse**(`response`, `json`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `Response` |
| `json` | `any` |

#### Returns

`void`

#### Defined in

src/classes/api/endpoints/GetGuildRequest.ts:30
