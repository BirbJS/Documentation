---
layout: default
title: RolePermissionOverwrite
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# RolePermissionOverwrite
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A RolePermissionOverwrite represents a role
overwrite for a channel on Discord.
# Constructor
```js
new RolePermissionOverwrite(client, role, allow, deny)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client this overwrite belongs to. | false | *none* |
| role | [Role](/ref/classes/Role) | The role this overwrite belongs to. | false | *none* |
| allow | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The allowed permissions. | false | 0 |
| deny | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The denied permissions.  | false | 0 |

# Properties
## allow
The allowed permissions.

**Type:** [PermissionsBlock](/ref/classes/PermissionsBlock)

## client
The client this overwrite belongs to.

**Type:** [Client](/ref/classes/Client)

## deny
The denied permissions.

**Type:** [PermissionsBlock](/ref/classes/PermissionsBlock)

## role
The role this overwrite belongs to.

**Type:** [Role](/ref/classes/Role)

# Methods
## grant(flags)
Grant the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to grant. | false | *none* |

**Returns:** [PermissionOverwrite](/ref/classes/PermissionOverwrite)

## revoke(flags)
Revoke the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to revoke. | false | *none* |

**Returns:** [PermissionOverwrite](/ref/classes/PermissionOverwrite)

