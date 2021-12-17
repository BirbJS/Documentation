---
layout: default
title: ClientUser
parent: Classes
has_children: false
has_toc: true
---

# ClientUser
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new ClientUser(client, data)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| data | any |  | false |  |

# Properties
## accent_color
**Type:** Object | string

## avatar
**Type:** Object | string

## banner
**Type:** Object | string

## bot
**Type:** boolean

## client
**Type:** [Client](classes/Client)

## discriminator
**Type:** string

## flags
**Type:** Object | string

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## system
**Type:** boolean

## tag
**Type:** string

## username
**Type:** string

# Methods
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

## setName(name)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string |  | false |  |

**Returns:** Promise<void>

## updatePresence(options)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | false |  |

**Returns:** void

