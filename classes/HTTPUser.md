---
layout: default
title: HTTPUser
parent: Classes
has_children: false
has_toc: true
---

# HTTPUser
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new HTTPUser()
```

# Methods
## createDM(client, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

## get(client, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

## getCurrent(client)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |

**Returns:** Promise<any>

## leaveGuild(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

## modifyCurrent(client, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

