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
| client | [Client](/classes/Client) |   | false | *none* |
| userId | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

**Returns:** Promise<any>

## get(client, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| userId | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

**Returns:** Promise<any>

## getCurrent(client)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |

**Returns:** Promise<any>

## leaveGuild(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

**Returns:** Promise<any>

## modifyCurrent(client, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

