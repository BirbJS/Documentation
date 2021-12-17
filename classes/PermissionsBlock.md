---
layout: default
title: PermissionsBlock
parent: Classes
has_children: false
has_toc: true
---

# PermissionsBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new PermissionsBlock(client, flags)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| flags | Object |  | false |  |

# Properties
## bits
**Type:** [Permissions](classes/Permissions)

## client
**Type:** [Client](classes/Client)

# Methods
## add(flags)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object |  | false |  |

**Returns:** [PermissionsBlock](classes/PermissionsBlock)

## equals(check)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| check | number | [PermissionsBlock](classes/PermissionsBlock) | [Permissions](classes/Permissions) |  | false |  |

**Returns:** boolean

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

**Returns:** [PermissionsBlock](classes/PermissionsBlock)

