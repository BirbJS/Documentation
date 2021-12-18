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
A Role represents a role in a guild on Discord.
# Constructor
```js
new Role(client, data, guild)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client that this Role belongs to. | false | *none* |
| data | any | The data of this Role. | false | *none* |
| guild | [Guild](/classes/Guild) | The guild this Role belongs to.
 | false | *none* |

# Properties
## client
The client that this Role belongs to.

**Type:** [Client](/classes/Client)

## color
The color of this Role as a hex color string.

**Type:** Object | string

## guild
The guild this Role belongs to.

**Type:** [Guild](/classes/Guild)

## hoist
Whether or not this Role is hoisted on the member
list.

**Type:** Object | boolean

## icon
The icon hash of this Role.

**Type:** Object | string

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this Role.

**Type:** string

## managed
Whether or not this Role is managed by Discord,
another application or a bot. If so, it cannot be
deleted.

**Type:** Object | boolean

## mentionable
Whether or not anyone can mention this Role.

**Type:** Object | boolean

## name
The name of this Role.

**Type:** Object | string

## permissions
The permissions of this Role.

**Type:** [RolePermissionsBlock](/classes/RolePermissionsBlock)

## position
The position of this Role.

**Type:** Object | number

## unicodeEmoji
The unicode emoji of this Role.

**Type:** Object | string

# Methods
## delete(reason?)
Delete this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | string |   | true | *none* |

**Returns:** Promise<void>

## modify(data, reason?)
Modify this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to modify this Role with. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## move(velocity, reason?)
Move this Role's position.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| velocity | number | The velocity to apply to this Role's position. Provide a positive integer to move this Role up, and a negative integer to move this Role down. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## setColor(color, reason?)
Set the color of this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| color | string | number | The new color for this Role. Accepts HEX color codes (e.g. ffffff for white) or an RGB integer. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## setIsHoisted(hoisted, reason?)
Set if this members of this Role should be hoisted
on the member list.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| hoisted | boolean | Whether or not this Role should be hoisted on the member list. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## setIsMentionable(mentionable, reason?)
Set if this Role can be mentioned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| mentionable | boolean | Whether or not this Role can be mentioned. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## setName(name, reason?)
Set the name of this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name to set this Role to. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## setPosition(position, reason?)
Set the position of this Role.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| position | number | The position to set this Role to. | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<[Role](/classes/Role)>

## toString()
Convert this Role into a mention (string).

**Returns:** string

## toIdOnly(role)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Convert a RoleResolvable into a role ID (string).

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| role | RoleResolvable | The Role to convert. | false | *none* |

**Returns:** string

