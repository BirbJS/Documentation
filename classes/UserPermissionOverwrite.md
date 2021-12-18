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
A UserPermissionOverwrite represents a user
overwrite for a channel on Discord.
# Constructor
```js
new UserPermissionOverwrite(client, user, allow, deny)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this overwrite belongs to. | false | *none* |
| user | [User](/classes/User) or [PartialUser](/classes/PartialUser) | The user this overwrite belongs to. | false | *none* |
| allow | number | The allowed permissions. | false | 0 |
| deny | number | The denied permissions.
 | false | 0 |

# Properties
## allow
The allowed permissions.

**Type:** [PermissionsBlock](/classes/PermissionsBlock)

## client
The client this overwrite belongs to.

**Type:** [Client](/classes/Client)

## deny
The denied permissions.

**Type:** [PermissionsBlock](/classes/PermissionsBlock)

## user
The user this overwrite belongs to.

**Type:** [User](/classes/User) or [PartialUser](/classes/PartialUser)

# Methods
## grant(flags)
Grant the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The flags to grant. | false | *none* |

**Returns:** [PermissionOverwrite](/classes/PermissionOverwrite)

## revoke(flags)
Revoke the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The flags to revoke. | false | *none* |

**Returns:** [PermissionOverwrite](/classes/PermissionOverwrite)

