---
layout: default
title: UserPermissionOverwrite
parent: Classes
grand_parent: Reference
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
| client | [Client](/ref/classes/Client) | The client this overwrite belongs to. | false | *none* |
| user | [User](/ref/classes/User) \| [PartialUser](/ref/classes/PartialUser) | The user this overwrite belongs to. | false | *none* |
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

## user
The user this overwrite belongs to.

**Type:** [User](/ref/classes/User) \| [PartialUser](/ref/classes/PartialUser)

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

