---
layout: default
title: GuildChannel
parent: Classes
has_children: false
has_toc: true
---

# GuildChannel
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildChannel(client, data, guild?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |
| guild | [Guild](/classes/Guild) |  | true |  |

# Properties
## client
**Type:** [Client](/classes/Client)

## guild
**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## name
**Type:** string

## permissions
**Type:** [ChannelPermissionsBlock](/classes/ChannelPermissionsBlock)

# Methods
## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** undefined | Object

## modify(data, reason?)
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[GuildChannel](/classes/GuildChannel)>

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | Object |  | false |  |

**Returns:** Promise<void>

