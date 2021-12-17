---
layout: default
title: BaseUser
parent: Classes
has_children: false
has_toc: true
---

# BaseUser
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new BaseUser(client, data)
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
## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

