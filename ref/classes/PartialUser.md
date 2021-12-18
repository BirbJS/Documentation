---
layout: default
title: PartialUser
parent: Classes
grand_parent: Reference
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
| client | [Client](/ref/classes/Client) | The client this user belongs to. | false | *none* |
| data | any | The data of this user.  | false | *none* |

# Properties
## client
**Type:** [Client](/ref/classes/Client)

## discriminator
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## tag
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## username
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## fetch(options?)
Fetch (and resolve) this PartialUser into a User.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** Promise<[User](/ref/classes/User)>

## isPartial()
Whether or not this instance is a full or partial
user. A partial user is a user that is only
guaranteed to have `id` set on them.

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## toString()
Convert this User into a mention (string).

**Returns:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

