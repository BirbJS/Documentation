---
layout: default
title: Role
parent: Classes
has_children: false
has_toc: true
---

# Role
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Role(client, data, guild)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |
| guild | [Guild](/classes/Guild) |  | false |  |

# Properties
## client
**Type:** [Client](/classes/Client)

## color
<<<<<<< Updated upstream
**Type:** Object | string
=======
The color of this Role as a hex color string.

**Type:** Object or string
>>>>>>> Stashed changes

## guild
**Type:** [Guild](/classes/Guild)

## hoist
<<<<<<< Updated upstream
**Type:** Object | boolean

## icon
**Type:** Object | string
=======
Whether or not this Role is hoisted on the member
list.

**Type:** Object or boolean

## icon
The icon hash of this Role.

**Type:** Object or string
>>>>>>> Stashed changes

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## managed
<<<<<<< Updated upstream
**Type:** Object | boolean

## mentionable
**Type:** Object | boolean

## name
**Type:** Object | string
=======
Whether or not this Role is managed by Discord,
another application or a bot. If so, it cannot be
deleted.

**Type:** Object or boolean

## mentionable
Whether or not anyone can mention this Role.

**Type:** Object or boolean

## name
The name of this Role.

**Type:** Object or string
>>>>>>> Stashed changes

## permissions
**Type:** [RolePermissionsBlock](/classes/RolePermissionsBlock)

## position
<<<<<<< Updated upstream
**Type:** Object | number

## unicodeEmoji
**Type:** Object | string
=======
The position of this Role.

**Type:** Object or number

## unicodeEmoji
The unicode emoji of this Role.

**Type:** Object or string
>>>>>>> Stashed changes

# Methods
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## delete(reason?)
Delete this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | string |  | true |  |

**Returns:** Promise<void>

## modify(data, reason?)
Modify this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to modify this Role with. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[Role](/classes/Role)>

## move(velocity, reason?)
Move this Role's position.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| velocity | number | The velocity to apply to this Role's position. Provide a positive integer to move this Role up, and a negative integer to move this Role down. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[Role](/classes/Role)>

## set()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Set the Role's data to the cache.

**Returns:** [Role](/classes/Role)

## setColor(color, reason?)
Set the color of this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
<<<<<<< Updated upstream
| color | string | number | The new color for this Role. Accepts HEX color codes (e.g. ffffff for white) or an RGB integer. | false |  |
| reason | string |  | true |  |
=======
| color | string or number | The new color for this Role. Accepts HEX color codes (e.g. ffffff for white) or an RGB integer. | false | *none* |
| reason | string |   | true | *none* |
>>>>>>> Stashed changes

**Returns:** Promise<[Role](/classes/Role)>

## setIsHoisted(hoisted, reason?)
Set if this members of this Role should be hoisted
on the member list.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| hoisted | boolean | Whether or not this Role should be hoisted on the member list. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[Role](/classes/Role)>

## setIsMentionable(mentionable, reason?)
Set if this Role can be mentioned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| mentionable | boolean | Whether or not this Role can be mentioned. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[Role](/classes/Role)>

## setName(name, reason?)
Set the name of this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name to set this Role to. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[Role](/classes/Role)>

## setPosition(position, reason?)
Set the position of this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| position | number | The position to set this Role to. | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[Role](/classes/Role)>

## toString()
Convert this Role into a mention (string).

**Returns:** string

## handleUpdate(client, data, guild)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PRIVATE
{: .label .label-red }

Handle updates from the Discord Gateway.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client that received the update. | false |  |
| data | any | The data to handle. | false |  |
| guild | [Guild](/classes/Guild) | The Guild this Role belongs to. | false |  |

**Returns:** [Role](/classes/Role)

## toIdOnly(role)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| role | RoleResolvable |  | false |  |

**Returns:** string

