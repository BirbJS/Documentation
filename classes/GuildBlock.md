---
layout: default
title: GuildBlock
parent: Classes
has_children: false
has_toc: true
---

# GuildBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A GuildBlock stores guild data.
# Constructor
```js
new GuildBlock(client, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| options | any |   | true | *none* |

# Properties
## cache
This block's cache.

**Type:** [Cache](/classes/Cache)

## client
The client that initilized this block.

**Type:** [Client](/classes/Client)

# Methods
## fetch(options)
Fetches a guild from the cache or Discord if it is
not already cached.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | GuildResolvable or *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The options to use. | false | *none* |

**Returns:** Promise<[Guild](/classes/Guild)>

