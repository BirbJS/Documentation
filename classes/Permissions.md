---
layout: default
title: Permissions
parent: Classes
has_children: false
has_toc: true
---

# Permissions
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Permissions objects store permission data.
# Constructor
```js
new Permissions(flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The permission flags.
 | false | *none* |

# Properties
## flags
The flags of the bitfield.

**Type:** number

## FLAGS
{: .d-inline-block }

STATIC
{: .label .label-blue }

The permission flags available.

**Type:** Object

# Methods
## add(flags)
Adds a flag (bit) to the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The flags to add. | false | *none* |

**Returns:** [BitsBlock](/classes/BitsBlock)

## clone()
Returns a new BitsBlock with the flags of this
block.

**Returns:** [BitsBlock](/classes/BitsBlock)

## has(flag)
Check if a flag (bit) is in the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flag | number | The flag to check. | false | *none* |

**Returns:** boolean

## hasPermission(flag)
Check whether or not the permission flags exist on
this Permissions object, whilst taking the
administrator permission into account. If you want
to ignore the administrator permission, use the
`has` method instead.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flag | number | The permission flag to check for. | false | *none* |

**Returns:** boolean

## isEmpty()
Check if the block is empty.

**Returns:** boolean

## remove(flags)
Removes a flag (bit) from the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The flags to remove. | false | *none* |

**Returns:** [BitsBlock](/classes/BitsBlock)

## set(flags)
Sets the flags of the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | number | The flags to set. | false | *none* |

**Returns:** [BitsBlock](/classes/BitsBlock)

