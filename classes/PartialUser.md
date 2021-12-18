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
**Warning:** Only the `id` property is guaranteed to be
set. Run the `fetch()` method to retrieve the entirety
of the User from the Discord API. If the username and/or
discriminator are not provided, they will be set to
`Unknown` and `0000` respectively.
# Constructor
```js
new PartialUser(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this user belongs to. | false | *none* |
| data | any | The data of this user.
 | false | *none* |

# Properties
## client
**Type:** [Client](/classes/Client)

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
## fetch(options?)
Fetch (and resolve) this PartialUser into a User.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |   | true | *none* |

**Returns:** Promise<[User](/classes/User)>

## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** boolean

## toString()
Convert this User into a mention (string).

**Returns:** string

