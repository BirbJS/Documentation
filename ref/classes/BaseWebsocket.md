---
layout: default
title: BaseWebsocket
parent: Classes
has_children: false
has_toc: true
---

# BaseWebsocket
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new BaseWebsocket(client, domain)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |
| domain | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

# Properties
## buffer
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** any

## client
**Type:** [Birb](/classes/Birb)

## domain
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## encoding
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## status
**Type:** [GatewayStatus](/enums/GatewayStatus)

## url
**Type:** URL

# Methods
## generateURL()
**Returns:** URL

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** void

## pack(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

## processPacket(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

## unpack(data, type?)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |
| type | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** any

