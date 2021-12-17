---
layout: default
title: RolePermissionsBlock
parent: Classes
has_children: false
has_toc: true
---

# RolePermissionsBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new RolePermissionsBlock(client, role, flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| role | [Role](/classes/Role) |  | false |  |
| flags | Object |  | false |  |

# Properties
## bits
**Type:** [Permissions](/classes/Permissions)

## client
**Type:** [Client](/classes/Client)

## role
**Type:** [Role](/classes/Role)

# Methods
## add(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [PermissionsBlock](/classes/PermissionsBlock)

## equals(check)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| check | number | [PermissionsBlock](/classes/PermissionsBlock) | [Permissions](/classes/Permissions) |  | false |  |

**Returns:** boolean

## grant(permissions, options)
Grant the role the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | number | Object | The permissions to grant. | false |  |
| options | Object | The options for the action. | false | {} |

**Returns:** Promise<[Role](/classes/Role)>

## has(flag, options)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flag | number |  | false |  |
| options | Object |  | false | ... |

**Returns:** boolean

## remove(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [PermissionsBlock](/classes/PermissionsBlock)

## revoke(permissions, options)
Revoke the specified permissions from the Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | number | Object | The permissions to revoke. | false |  |
| options | Object | The options for the action. | false | {} |

**Returns:** Promise<[Role](/classes/Role)>

## set(permissions, options)
Set the permissions for the Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | number | Object | The permissions to set. | false |  |
| options | Object | The options for the action. | false | {} |

**Returns:** Promise<[Role](/classes/Role)>

