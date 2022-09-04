---
layout: default
title: ModifyGuildRequest
parent: Classes
has_children: false
has_toc: true
---

# ModifyGuildRequest
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new ModifyGuildRequest(client)
```

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| client | [Birb](/classes/Birb) |   | *none* |

# Properties
## body
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| ModifyGuildRequestBody

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
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| ModifyGuildParams

# Methods
## buildURL(params)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| params | ModifyGuildParams |   | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## execute()
**Returns:** Promise<APIResponse<APIGuild>>

## furnishRequest()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setAuditLogReason(reason?)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| reason? | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setBody(body)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| body | *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| ModifyGuildRequestBody |   | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setHeaders(headers)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| headers | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setParams(params)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| params | ModifyGuildParams |   | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## throwJSONError(response, json?)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| response | Response |   | *none* |
| json? | any |   | *none* |

**Returns:** [BirbAPIError](/classes/BirbAPIError)

