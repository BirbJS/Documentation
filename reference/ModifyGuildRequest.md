---
layout: default
title: ModifyGuildRequest
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / ModifyGuildRequest

# Class: ModifyGuildRequest

## Hierarchy

- [`AuthenticatedAPIEndpoint`](AuthenticatedAPIEndpoint.md)<[`ModifyGuildParams`](modules.md#modifyguildparams), [`APIGuild`](modules.md#apiguild), [`ModifyGuildRequestBody`](modules.md#modifyguildrequestbody)\>

  ↳ **`ModifyGuildRequest`**

## Table of contents

### Constructors

- [constructor](ModifyGuildRequest.md#constructor)

### Properties

- [body](ModifyGuildRequest.md#body)
- [client](ModifyGuildRequest.md#client)
- [headers](ModifyGuildRequest.md#headers)
- [method](ModifyGuildRequest.md#method)
- [params](ModifyGuildRequest.md#params)

### Methods

- [buildURL](ModifyGuildRequest.md#buildurl)
- [execute](ModifyGuildRequest.md#execute)
- [furnishRequest](ModifyGuildRequest.md#furnishrequest)
- [setAuditLogReason](ModifyGuildRequest.md#setauditlogreason)
- [setBody](ModifyGuildRequest.md#setbody)
- [setHeaders](ModifyGuildRequest.md#setheaders)
- [setParams](ModifyGuildRequest.md#setparams)
- [throwJSONError](ModifyGuildRequest.md#throwjsonerror)

## Constructors

### constructor

• **new ModifyGuildRequest**(`client`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |

#### Overrides

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[constructor](AuthenticatedAPIEndpoint.md#constructor)

#### Defined in

src/classes/api/endpoints/ModifyGuildRequest.ts:38

## Properties

### body

• **body**: `undefined` \| [`ModifyGuildRequestBody`](modules.md#modifyguildrequestbody)

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

• **params**: `undefined` \| [`ModifyGuildParams`](modules.md#modifyguildparams)

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
| `params` | [`ModifyGuildParams`](modules.md#modifyguildparams) |

#### Returns

`string`

#### Overrides

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[buildURL](AuthenticatedAPIEndpoint.md#buildurl)

#### Defined in

src/classes/api/endpoints/ModifyGuildRequest.ts:42

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

▸ `Protected` **furnishRequest**(): [`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Returns

[`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[furnishRequest](AuthenticatedAPIEndpoint.md#furnishrequest)

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:9

___

### setAuditLogReason

▸ **setAuditLogReason**(`reason?`): [`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `string` |

#### Returns

[`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setAuditLogReason](AuthenticatedAPIEndpoint.md#setauditlogreason)

#### Defined in

src/classes/api/AuthenticatedAPIEndpoint.ts:20

___

### setBody

▸ **setBody**(`body`): [`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `undefined` \| [`ModifyGuildRequestBody`](modules.md#modifyguildrequestbody) |

#### Returns

[`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setBody](AuthenticatedAPIEndpoint.md#setbody)

#### Defined in

src/classes/api/APIEndpoint.ts:46

___

### setHeaders

▸ **setHeaders**(`headers`): [`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers` | `Object` |

#### Returns

[`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Inherited from

[AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint.md).[setHeaders](AuthenticatedAPIEndpoint.md#setheaders)

#### Defined in

src/classes/api/APIEndpoint.ts:36

___

### setParams

▸ **setParams**(`params`): [`ModifyGuildRequest`](ModifyGuildRequest.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`ModifyGuildParams`](modules.md#modifyguildparams) |

#### Returns

[`ModifyGuildRequest`](ModifyGuildRequest.md)

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
