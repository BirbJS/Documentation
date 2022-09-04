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

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |

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
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| params | ModifyGuildParams |   | false | *none* |

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## execute()
**Returns:** Promise<APIResponse<APIGuild>>

## furnishRequest()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setAuditLogReason(reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setBody(body)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| body | *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| ModifyGuildRequestBody |   | false | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setHeaders(headers)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| headers | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## setParams(params)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| params | ModifyGuildParams |   | false | *none* |

**Returns:** [ModifyGuildRequest](/classes/ModifyGuildRequest)

## throwJSONError(response, json?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| response | Response |   | false | *none* |
| json | any |   | true | *none* |

**Returns:** [BirbAPIError](/classes/BirbAPIError)

