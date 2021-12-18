---
layout: default
title: UserBlock
parent: Classes
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
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| options | any |   | true | *none* |

# Properties
## cache
This block's cache.

**Type:** [Cache](/classes/Cache)

## client
The client that initilized this block.

**Type:** [Client](/classes/Client)

# Methods
## fetch(userId, options?)
Fetches a user from the Cache or the Discord API if
the user is not cached.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| userId | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The ID of the user to fetch. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** Promise<[User](/classes/User)>

## fetchMe()
Fetches this Client's user.

**Returns:** Promise<[ClientUser](/classes/ClientUser)>

## resolve(user, def?)
Resolves a UserResolvable to a user if the user is
in the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable | The user to resolve. | false | *none* |
| def | any |   | true | *none* |

**Returns:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* or [User](/classes/User)

