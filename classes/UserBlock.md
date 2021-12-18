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
# Constructor
```js
new UserBlock(client, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| options | any |  | true |  |

# Properties
## cache
**Type:** [Cache](/classes/Cache)

## client
**Type:** [Client](/classes/Client)

# Methods
## fetch(userId, options?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| userId | string |  | false |  |
| options | Object |  | true |  |

**Returns:** Promise<[User](/classes/User)>

## fetchMe()
**Returns:** Promise<[ClientUser](/classes/ClientUser)>

## resolve(user, def?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable |  | false |  |
| def | any |  | true |  |

**Returns:** Object or [User](/classes/User)

