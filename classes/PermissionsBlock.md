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
The PermissionsBlock stores permissions data.
# Constructor
```js
new PermissionsBlock(client, flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| flags | Object |   | false | *none* |

# Properties
## bits
The permissions bits.

**Type:** [Permissions](/classes/Permissions)

## client
The client that initiliazed the block.

**Type:** [Client](/classes/Client)

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

