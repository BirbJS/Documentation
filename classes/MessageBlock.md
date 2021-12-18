---
layout: default
title: MessageBlock
parent: Classes
has_children: false
has_toc: true
---

# MessageBlock
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A MessageBlock stores information on messages.
# Constructor
```js
new MessageBlock(client, guild, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| guild | [Guild](/classes/Guild) | The guild instance. | false | *none* |
| options | any |   | true | *none* |

# Properties
## cache
This block's cache.

**Type:** [Cache](/classes/Cache)

## client
The client that initilized this block.

**Type:** [Client](/classes/Client)

