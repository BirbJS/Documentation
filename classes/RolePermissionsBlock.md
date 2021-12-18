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
A RolePermissionsBlock stores role permissions data.
# Constructor
```js
new RolePermissionsBlock(client, role, flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| role | [Role](/classes/Role) | The Role this PermissionsBlock is for. | false | *none* |
| flags | Object | The permissions to set.
 | false | *none* |

# Properties
## bits
The permissions bits.

**Type:** [Permissions](/classes/Permissions)

## client
The client that initiliazed the block.

**Type:** [Client](/classes/Client)

## role
The Role this PermissionsBlock is for.

**Type:** [Role](/classes/Role)

# Methods
## add(flags)
Add a permission bit.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The permission bit. | false | *none* |

**Returns:** [PermissionsBlock](/classes/PermissionsBlock)

## equals(check)
Compare the PermissionsBlock to another PermissionsBlock.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| check | number or [PermissionsBlock](/classes/PermissionsBlock) or [Permissions](/classes/Permissions) | The PermissionsBlock or Permissions to compare to. | false | *none* |

**Returns:** boolean

## grant(permissions, options)
Grant the role the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | number or Object | The permissions to grant. | false | *none* |
| options | Object | The options for the action. | false | {} |

**Returns:** Promise<[Role](/classes/Role)>

## has(flag, options)
Check if the PermissionsBlock has a permission bit.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flag | number | The permission bit. | false | *none* |
| options | Object |   | false | ... |

**Returns:** boolean

## remove(flags)
Remove a permission bit.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The permission bit. | false | *none* |

**Returns:** [PermissionsBlock](/classes/PermissionsBlock)

## revoke(permissions, options)
Revoke the specified permissions from the Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | number or Object | The permissions to revoke. | false | *none* |
| options | Object | The options for the action. | false | {} |

**Returns:** Promise<[Role](/classes/Role)>

## set(permissions, options)
Set the permissions for the Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | number or Object | The permissions to set. | false | *none* |
| options | Object | The options for the action. | false | {} |

**Returns:** Promise<[Role](/classes/Role)>

