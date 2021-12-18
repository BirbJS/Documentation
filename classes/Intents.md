---
layout: default
title: Intents
parent: Classes
has_children: false
has_toc: true
---

# Intents
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Intents are used by Discord to selectively send the
client data, whilst not sending data that isn't
needed. Intents are required to be set to use
Birb.JS.
# Constructor
```js
new Intents(flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | Object | The flags to set.
 | false | *none* |

# Properties
## flags
The flags of the bitfield.

**Type:** number

## FLAGS
{: .d-inline-block }

STATIC
{: .label .label-blue }

The available Intents.

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

