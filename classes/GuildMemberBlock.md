---
layout: default
title: GuildMemberBlock
parent: Classes
has_children: false
has_toc: true
---

# GuildMemberBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildMemberBlock(client, guild, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| guild | [Guild](/classes/Guild) |  | false |  |
| options | any |  | true |  |

# Properties
## cache
**Type:** [Cache](/classes/Cache)

## client
**Type:** [Client](/classes/Client)

## guild
**Type:** [Guild](/classes/Guild)

# Methods
## fetch(userId, options?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| userId | string |  | false |  |
| options | Object |  | true |  |

**Returns:** Promise<[GuildMember](/classes/GuildMember)>

## resolve(user, guild, def?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| user | UserResolvable |  | false |  |
| guild | [Guild](/classes/Guild) |  | false |  |
| def | any |  | true |  |

**Returns:** Object or [GuildMember](/classes/GuildMember)

