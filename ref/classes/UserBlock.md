---
layout: default
title: UserBlock
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# UserBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A UserBlock stores user data.
# Constructor
```js
new UserBlock(client, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client instance. | false | *none* |
| options | any |   | true | *none* |

# Properties
## cache
This block's cache.

**Type:** [Cache](/ref/classes/Cache)

## client
The client that initilized this block.

**Type:** [Client](/ref/classes/Client)

# Methods
## fetch(userId, options?)
Fetches a user from the Cache or the Discord API if
the user is not cached.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| userId | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The ID of the user to fetch. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** Promise<[User](/ref/classes/User)>

## fetchMe()
Fetches this Client's user.

**Returns:** Promise<[ClientUser](/ref/classes/ClientUser)>

## resolve(user, def?)
Resolves a UserResolvable to a user if the user is
in the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable | The user to resolve. | false | *none* |
| def | any |   | true | *none* |

**Returns:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| [User](/ref/classes/User)

