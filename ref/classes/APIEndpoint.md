---
layout: default
title: APIEndpoint
parent: Classes
has_children: false
has_toc: true
---

# APIEndpoint
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new APIEndpoint(client, method)
```

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| client | [Birb](/classes/Birb) |   | *none* |
| method | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | *none* |

# Properties
## body
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| Body

## client
**Type:** [Birb](/classes/Birb)

## headers
**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## method
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## params
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| Params

# Methods
## buildURL(params)
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| params | Params |   | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## execute()
**Returns:** Promise<APIResponse<Response>>

## setBody(body)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| body | *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| Body |   | *none* |

**Returns:** APIEndpoint<Params, Response, Body>

## setHeaders(headers)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| headers | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** APIEndpoint<Params, Response, Body>

## setParams(params)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| params | Params |   | *none* |

**Returns:** APIEndpoint<Params, Response, Body>

## throwJSONError(response, json?)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| response | Response |   | *none* |
| json? | any |   | *none* |

**Returns:** [BirbAPIError](/classes/BirbAPIError)

