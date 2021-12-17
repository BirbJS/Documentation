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
# Constructor
```js
new PermissionOverwrite(client, allow, deny)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| allow | number |  | false | 0 |
| deny | number |  | false | 0 |

# Properties
## allow
**Type:** [PermissionsBlock](classes/PermissionsBlock)

## client
**Type:** [Client](classes/Client)

## deny
**Type:** [PermissionsBlock](classes/PermissionsBlock)

# Methods
## grant(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [PermissionOverwrite](classes/PermissionOverwrite)

## revoke(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [PermissionOverwrite](classes/PermissionOverwrite)

