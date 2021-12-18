---
layout: default
title: PermissionOverwrite
parent: Classes
has_children: false
has_toc: true
---

# PermissionOverwrite
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A permission overwrite represents a user or role
overwrite for a channel.
# Constructor
```js
new PermissionOverwrite(client, allow, deny)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this overwrite belongs to. | false | *none* |
| allow | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The allowed permissions. | false | 0 |
| deny | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The denied permissions.  | false | 0 |

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

# Methods
## grant(flags)
Grant the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to grant. | false | *none* |

**Returns:** [PermissionOverwrite](/classes/PermissionOverwrite)

## revoke(flags)
Revoke the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to revoke. | false | *none* |

**Returns:** [PermissionOverwrite](/classes/PermissionOverwrite)

