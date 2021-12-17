---
layout: default
title: UserPermissionOverwrite
parent: Classes
has_children: false
has_toc: true
---

# UserPermissionOverwrite
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new UserPermissionOverwrite(client, user, allow, deny)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| user | [User](classes/User) | [PartialUser](classes/PartialUser) |  | false |  |
| allow | number |  | false | 0 |
| deny | number |  | false | 0 |

# Properties
## allow
**Type:** [PermissionsBlock](classes/PermissionsBlock)

## client
**Type:** [Client](classes/Client)

## deny
**Type:** [PermissionsBlock](classes/PermissionsBlock)

## user
**Type:** [User](classes/User) | [PartialUser](classes/PartialUser)

# Methods
## grant(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [UserPermissionOverwrite](classes/UserPermissionOverwrite)

## revoke(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [UserPermissionOverwrite](classes/UserPermissionOverwrite)

