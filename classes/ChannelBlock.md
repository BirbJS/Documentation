---
layout: default
title: ChannelBlock
parent: Classes
has_children: false
has_toc: true
---

# ChannelBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A ChannelBlock stores channel data.
# Constructor
```js
new ChannelBlock(client, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| options | any |   | true | *none* |

# Properties
## cache
The cache full of channels.

**Type:** [CCache](/classes/CCache)

## client
The client that initilized this block.

**Type:** [Client](/classes/Client)

