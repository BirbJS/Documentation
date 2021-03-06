---
layout: default
title: PermissionsBlock
parent: Classes
grand_parent: Reference
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
| client | [Client](/ref/classes/Client) | The client instance. | false | *none* |
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

# Properties
## bits
The permissions bits.

**Type:** [Permissions](/ref/classes/Permissions)

## client
The client that initiliazed the block.

**Type:** [Client](/ref/classes/Client)

# Methods
## add(flags)
Add a permission bit.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The permission bit. | false | *none* |

**Returns:** [PermissionsBlock](/ref/classes/PermissionsBlock)

## equals(check)
Compare the PermissionsBlock to another PermissionsBlock.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| check | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| [PermissionsBlock](/ref/classes/PermissionsBlock) \| [Permissions](/ref/classes/Permissions) | The PermissionsBlock or Permissions to compare to. | false | *none* |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## has(flag, options)
Check if the PermissionsBlock has a permission bit.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flag | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The permission bit. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | ... |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## remove(flags)
Remove a permission bit.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The permission bit. | false | *none* |

**Returns:** [PermissionsBlock](/ref/classes/PermissionsBlock)

