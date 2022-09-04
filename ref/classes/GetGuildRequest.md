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

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| client | [Birb](/classes/Birb) |   | *none* |

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
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| params | GetGuildParams |   | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## execute()
**Returns:** Promise<APIResponse<APIGuild>>

## furnishRequest()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setAuditLogReason(reason?)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| reason? | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setBody(body)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| body | any |   | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setHeaders(headers)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| headers | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## setParams(params)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| params | GetGuildParams |   | *none* |

**Returns:** [GetGuildRequest](/classes/GetGuildRequest)

## throwJSONError(response, json?)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| response | Response |   | *none* |
| json? | any |   | *none* |

**Returns:** [BirbAPIError](/classes/BirbAPIError)

## validateResponse(response, json)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| response | Response |   | *none* |
| json | any |   | *none* |

**Returns:** void

