---
layout: default
title: Request
parent: Classes
has_children: false
has_toc: true
---

# Request
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Request(client, method, path, body?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| method | HTTPMethod |   | false | *none* |
| path | string |   | false | *none* |
| body | any |   | true | *none* |

# Properties
## body
**Type:** any

## client
**Type:** [Client](/classes/Client)

## method
**Type:** HTTPMethod

## reason
**Type:** Object | string

## response
**Type:** any

## upload
**Type:** boolean

## url
**Type:** string

# Methods
## make(files?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| files | Object |   | true | *none* |

**Returns:** Promise<any>

