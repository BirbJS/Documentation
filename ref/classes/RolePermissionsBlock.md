---
layout: default
title: RolePermissionsBlock
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# RolePermissionsBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A RolePermissionsBlock stores role permissions data.
# Constructor
```js
new RolePermissionsBlock(client, role, flags)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client instance. | false | *none* |
| role | [Role](/ref/classes/Role) | The Role this PermissionsBlock is for. | false | *none* |
| flags | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The permissions to set.  | false | *none* |

# Properties
## bits
The permissions bits.

**Type:** [Permissions](/ref/classes/Permissions)

## client
The client that initiliazed the block.

**Type:** [Client](/ref/classes/Client)

## role
The Role this PermissionsBlock is for.

**Type:** [Role](/ref/classes/Role)

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

## grant(permissions, options)
Grant the role the specified permissions.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The permissions to grant. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The options for the action. | false | {} |

**Returns:** Promise<[Role](/ref/classes/Role)>

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

## revoke(permissions, options)
Revoke the specified permissions from the Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The permissions to revoke. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The options for the action. | false | {} |

**Returns:** Promise<[Role](/ref/classes/Role)>

## set(permissions, options)
Set the permissions for the Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| permissions | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The permissions to set. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The options for the action. | false | {} |

**Returns:** Promise<[Role](/ref/classes/Role)>

