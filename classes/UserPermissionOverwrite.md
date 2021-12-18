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
<<<<<<< Updated upstream
| client | [Client](/classes/Client) |  | false |  |
| user | [User](/classes/User) | [PartialUser](/classes/PartialUser) |  | false |  |
| allow | number |  | false | 0 |
| deny | number |  | false | 0 |
=======
| client | [Client](/classes/Client) | The client this overwrite belongs to. | false | *none* |
| user | [User](/classes/User) or [PartialUser](/classes/PartialUser) | The user this overwrite belongs to. | false | *none* |
| allow | number | The allowed permissions. | false | 0 |
| deny | number | The denied permissions.
 | false | 0 |
>>>>>>> Stashed changes

# Properties
## allow
**Type:** [PermissionsBlock](/classes/PermissionsBlock)

## client
**Type:** [Client](/classes/Client)

## deny
**Type:** [PermissionsBlock](/classes/PermissionsBlock)

## user
<<<<<<< Updated upstream
**Type:** [User](/classes/User) | [PartialUser](/classes/PartialUser)
=======
The user this overwrite belongs to.

**Type:** [User](/classes/User) or [PartialUser](/classes/PartialUser)
>>>>>>> Stashed changes

# Methods
## grant(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [UserPermissionOverwrite](/classes/UserPermissionOverwrite)

## revoke(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [UserPermissionOverwrite](/classes/UserPermissionOverwrite)

