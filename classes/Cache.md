---
layout: default
title: Cache
parent: Classes
has_children: false
has_toc: true
---

# Cache
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Cache(options?)
```
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | Object |  | true |  |

# Properties
## cache
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Type:** Map<string, any>

## client
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

**Type:** [Client](classes/Client)

## options
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Type:** any

# Methods
## array()
Get an array of the entries in the cache.

**Returns:** Object

## arrayPair()
Get an array of the entries in the cache as `Pair`s.

**Returns:** Object

## clear()
Clear the cache and its contents.

**Returns:** [Cache](classes/Cache)

## entries()
Get an object of the entries in the cache. The
key is the key of the entry, and the value is
the value of the entry.

**Returns:** Object

## filter(fn)
Filter values in the cache. If the key is not found
in the cache, an empty array is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | Object |  | false |  |

**Returns:** Object

## find(fn)
Find a value in the cache. If the key is not found
in the cache, `null` is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | Object |  | false |  |

**Returns:** any

## get(key)
Get a value from the cache. If the key is not found
in the cache, `null` is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key to get the value for. | false |  |

**Returns:** any

## has(key)
Check if the cache contains a key.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key of the entry. | false |  |

**Returns:** boolean

## makeSpace(options?)
Make space in the cache for a new entry. You
**probably shouldn't** run this method directly
unless you know **EXACTLY** what you're doing.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | any |  | true |  |

**Returns:** void

## rebuild(data)
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** any

## remove(key)
Remove a key from the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key of the entry. | false |  |

**Returns:** [Cache](classes/Cache)

## set(key, value, options?)
Set a value in the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key of the entry. | false |  |
| value | any | The value to set it to. | false |  |
| options | any |  | true |  |

**Returns:** [Cache](classes/Cache)

## size()
Get the amount of entries in the cache.

**Returns:** number

## strip(data)
{: .d-inline-block }

ABSTRACT
{: .label .label-yellow }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** any

