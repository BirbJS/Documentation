---
layout: default
title: CCache
parent: Classes
has_children: false
has_toc: true
---

# CCache
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Creates a new CCache instance.
# Constructor
```js
new CCache(client, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| options | Object |   | true | *none* |

# Properties
## client
The Client that initialized the cache.

**Type:** [Client](/classes/Client)

# Methods
## array()
Get an array of the entries in the cache.

**Returns:** Object

## arrayPair()
Get an array of the entries in the cache as `Pair`s.

**Returns:** Object

## clear()
Clear the cache and its contents.

**Returns:** [Cache](/classes/Cache)

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
| fn | Object |   | false | *none* |

**Returns:** Object

## find(fn)
Find a value in the cache. If the key is not found
in the cache, `null` is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | Object |   | false | *none* |

**Returns:** any

## get(key)
Get a value from the cache. If the key is not found
in the cache, `null` is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key to get the value for. | false | *none* |

**Returns:** any

## has(key)
Check if the cache contains a key.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key of the entry. | false | *none* |

**Returns:** boolean

## makeSpace(options?)
Make space in the cache for a new entry. You
**probably shouldn't** run this method directly
unless you know **EXACTLY** what you're doing.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | any |   | true | *none* |

**Returns:** void

## rebuild(data)
A method called to rebuild data that has been
stripped.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

## remove(key)
Remove a key from the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key of the entry. | false | *none* |

**Returns:** [Cache](/classes/Cache)

## set(key, value, options?)
Set a value in the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | string | The key of the entry. | false | *none* |
| value | any | The value to set it to. | false | *none* |
| options | any |   | true | *none* |

**Returns:** [Cache](/classes/Cache)

## size()
Get the amount of entries in the cache.

**Returns:** number

## strip(data)
A method called to strip unwanted properties from an
entry before it is added to the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

