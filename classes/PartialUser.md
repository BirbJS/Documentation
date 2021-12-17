---
layout: default
title: PartialUser
parent: Classes
has_children: false
has_toc: true
---

# PartialUser
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new PartialUser(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| data | any |  | false |  |

# Properties
## client
**Type:** [Client](classes/Client)

## discriminator
**Type:** string

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

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

## fetch(options?)
Fetch (and resolve) this PartialUser into a User.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | true |  |

**Returns:** Promise<[User](classes/User)>

## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

## toString()
Convert this User into a mention (string).

**Returns:** string

