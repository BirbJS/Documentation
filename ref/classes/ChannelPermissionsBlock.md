---
layout: default
title: ChannelPermissionsBlock
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# ChannelPermissionsBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A ChannelPermissionsBlock stores data about channel
permissions.
# Constructor
```js
new ChannelPermissionsBlock(client, channel, overwrites)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client instance. | false | *none* |
| channel | [GuildChannel](/ref/classes/GuildChannel) | The channel this permissions block is for. | false | *none* |
| overwrites | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The data to parse.  | false | *none* |

# Properties
## channel
The channel this permissions block is for.

**Type:** [GuildChannel](/ref/classes/GuildChannel)

## client
The client that initiliazed the block.

**Type:** [Client](/ref/classes/Client)

## overwrites
The list of permission overwrites.

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

