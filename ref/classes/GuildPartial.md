---
layout: default
title: GuildPartial
parent: Classes
has_children: false
has_toc: true
---

# GuildPartial
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildPartial(client, guild)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |
| guild | APIGuild \| APIGuildPartial |   | false | *none* |

# Properties
## available
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## client
**Type:** [Birb](/classes/Birb)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## fetch()
**Returns:** Promise<[Guild](/classes/Guild)>

## isPartial()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

