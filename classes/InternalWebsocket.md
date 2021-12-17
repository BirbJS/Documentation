---
layout: default
title: InternalWebsocket
parent: Classes
has_children: false
has_toc: true
---

# InternalWebsocket
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
## Constructor
```js
new InternalWebsocket(client, domain)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| domain | string |  | false |  |

## Properties
### buffer
**Type:** any

### client
**Type:** [Client](classes/Client)

### domain
**Type:** string

### encoding
**Type:** string

### status
**Type:** [WebsocketStatus](enums/WebsocketStatus)

### url
**Type:** URL

## Methods
### generateURL()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** URL

### init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** void

### pack(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** any

### processPacket(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** any

### unpack(data, type?)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |
| type | string |  | true |  |

**Returns:** any

