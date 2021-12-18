---
layout: default
title: BitsBlock
parent: Classes
has_children: false
has_toc: true
---

# BitsBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A BitsBlock stores bitfield data provided by Discord.
# Constructor
```js
new BitsBlock(flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to set.
 | false | *none* |

# Properties
## flags
The flags of the bitfield.

**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

# Methods
## add(flags)
Adds a flag (bit) to the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to add. | false | *none* |

**Returns:** [BitsBlock](/classes/BitsBlock)

## clone()
Returns a new BitsBlock with the flags of this
block.

**Returns:** [BitsBlock](/classes/BitsBlock)

## has(flag)
Check if a flag (bit) is in the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flag | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The flag to check. | false | *none* |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isEmpty()
Check if the block is empty.

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## remove(flags)
Removes a flag (bit) from the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The flags to remove. | false | *none* |

**Returns:** [BitsBlock](/classes/BitsBlock)

## set(flags)
Sets the flags of the block.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The flags to set. | false | *none* |

**Returns:** [BitsBlock](/classes/BitsBlock)

