---
layout: default
title: GuildMemberBlock
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# GuildMemberBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A GuildMemberBlock stores guild member data.
# Constructor
```js
new GuildMemberBlock(client, guild, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client instance. | false | *none* |
| guild | [Guild](/ref/classes/Guild) | The guild that the block is for. | false | *none* |
| options | any |   | true | *none* |

# Properties
## cache
This block's cache.

**Type:** [Cache](/ref/classes/Cache)

## client
The client that initilized this block.

**Type:** [Client](/ref/classes/Client)

## guild
The guild that the block is for.

**Type:** [Guild](/ref/classes/Guild)

# Methods
## fetch(userId, options?)
Fetch a guild member from the cache or the Discord\
API if it is not in the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| userId | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The user's ID. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

**Returns:** Promise<[GuildMember](/ref/classes/GuildMember)>

## resolve(user, def?)
Resolve a user to a GuildMember. Returns null if the
member is not cached.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable | The member to resolve. | false | *none* |
| def | any |   | true | *none* |

**Returns:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| [GuildMember](/ref/classes/GuildMember)

