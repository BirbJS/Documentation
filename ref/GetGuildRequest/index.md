---
layout: default
title: "GetGuildRequest"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / GetGuildRequest

# Class: GetGuildRequest

## Hierarchy

- [`AuthenticatedAPIEndpoint`](../AuthenticatedAPIEndpoint/index.md)<[`GetGuildParams`](../modules.md#getguildparams), [`APIGuild`](../modules.md#apiguild)\>

  ↳ **`GetGuildRequest`**

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
- [validateResponse](index.md#validateresponse)

## Constructors

### constructor

• **new GetGuildRequest**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |

#### Overrides

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[constructor](../AuthenticatedAPIEndpoint/index.md#constructor)

#### Defined in

src/classes/api/endpoints/GetGuildRequest.ts:16

## Properties

### body

• **body**: `any`

The request body.

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[body](../AuthenticatedAPIEndpoint/index.md#body)

#### Defined in

src/classes/api/APIEndpoint.ts:29

___

### client

• **client**: [`Birb`](../Birb/index.md)

The Birb client.

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[client](../AuthenticatedAPIEndpoint/index.md#client)

#### Defined in

src/classes/api/APIEndpoint.ts:10

___

### headers

• **headers**: `Object`

The parameters to use.

#### Index signature

▪ [key: `string`]: `string`

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[headers](../AuthenticatedAPIEndpoint/index.md#headers)

#### Defined in

src/classes/api/APIEndpoint.ts:22

___

### method

• `Readonly` **method**: `string`

The method for the endpoint.

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[method](../AuthenticatedAPIEndpoint/index.md#method)

#### Defined in

src/classes/api/APIEndpoint.ts:14

___

### params

• **params**: `undefined` \| [`GetGuildParams`](../modules.md#getguildparams)

The parameters to use.

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[params](../AuthenticatedAPIEndpoint/index.md#params)

#### Defined in

src/classes/api/APIEndpoint.ts:18

## Methods

### buildURL

▸ **buildURL**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`GetGuildParams`](../modules.md#getguildparams) |

#### Returns

`string`

#### Overrides

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[buildURL](../AuthenticatedAPIEndpoint/index.md#buildurl)

#### Defined in

src/classes/api/endpoints/GetGuildRequest.ts:20

___

### execute

▸ **execute**(): `Promise`<[`APIResponse`](../modules.md#apiresponse)<[`APIGuild`](../modules.md#apiguild)\>\>

#### Returns

`Promise`<[`APIResponse`](../modules.md#apiresponse)<[`APIGuild`](../modules.md#apiguild)\>\>

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[execute](../AuthenticatedAPIEndpoint/index.md#execute)

#### Defined in

src/classes/api/APIEndpoint.ts:51

___

### furnishRequest

▸ `Protected` **furnishRequest**(): [`GetGuildRequest`](index.md)

#### Returns

[`GetGuildRequest`](index.md)

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[furnishRequest](../AuthenticatedAPIEndpoint/index.md#furnishrequest)

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:9

___

### setAuditLogReason

▸ **setAuditLogReason**(`reason?`): [`GetGuildRequest`](index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `string` |

#### Returns

[`GetGuildRequest`](index.md)

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[setAuditLogReason](../AuthenticatedAPIEndpoint/index.md#setauditlogreason)

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:20

___

### setBody

▸ **setBody**(`body`): [`GetGuildRequest`](index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `any` |

#### Returns

[`GetGuildRequest`](index.md)

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[setBody](../AuthenticatedAPIEndpoint/index.md#setbody)

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`GetGuildRequest`](index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`GetGuildRequest`](index.md)

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[setHeaders](../AuthenticatedAPIEndpoint/index.md#setheaders)

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`GetGuildRequest`](index.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`GetGuildParams`](../modules.md#getguildparams) |

#### Returns

[`GetGuildRequest`](index.md)

#### Inherited from

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[setParams](../AuthenticatedAPIEndpoint/index.md#setparams)

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

[AuthenticatedAPIEndpoint](../AuthenticatedAPIEndpoint/index.md).[throwJSONError](../AuthenticatedAPIEndpoint/index.md#throwjsonerror)

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
