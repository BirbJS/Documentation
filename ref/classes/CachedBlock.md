---
layout: default
title: CachedBlock
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# CachedBlock
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A CachedBlock is the base class for all blocks that
cache data.
# Constructor
```js
new CachedBlock(client, cache)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client to use. | false | *none* |
| cache | [Cache](/ref/classes/Cache) | The cache to use.  | false | *none* |

# Properties
## cache
This block's cache.

**Type:** [Cache](/ref/classes/Cache)

## client
The client that initilized this block.

**Type:** [Client](/ref/classes/Client)

