---
layout: default
title: GetGuildRequest
parent: Classes
has_children: false
has_toc: true
---

# GetGuildRequest
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GetGuildRequest(client)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |

# Properties
## body
**Type:** any

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
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| GetGuildParams

# Methods
## buildURL(params)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| params | GetGuildParams |   | false | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## execute()
**Returns:** Promise<APIResponse<APIGuild>>

## furnishRequest()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setAuditLogReason(reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setBody(body)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| body | any |   | false | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setHeaders(headers)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| headers | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setParams(params)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| params | GetGuildParams |   | false | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## throwJSONError(response, json?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| response | Response |   | false | *none* |
| json | any |   | true | *none* |

**Returns:** [BirbAPIError](/classes/BirbAPIError)

## validateResponse(response, json)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| response | Response |   | false | *none* |
| json | any |   | false | *none* |

**Returns:** void

