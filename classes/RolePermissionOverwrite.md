---
layout: default
title: RolePermissionOverwrite
parent: Classes
has_children: false
has_toc: true
---

# RolePermissionOverwrite
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
## Constructor
```js
new RolePermissionOverwrite(client, role, allow, deny)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| role | [Role](classes/Role) |  | false |  |
| allow | number |  | false | 0 |
| deny | number |  | false | 0 |

## Properties
### allow
**Type:** [PermissionsBlock](classes/PermissionsBlock)

### client
**Type:** [Client](classes/Client)

### deny
**Type:** [PermissionsBlock](classes/PermissionsBlock)

### role
**Type:** [Role](classes/Role)

## Methods
### grant(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [RolePermissionOverwrite](classes/RolePermissionOverwrite)

### revoke(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [RolePermissionOverwrite](classes/RolePermissionOverwrite)

