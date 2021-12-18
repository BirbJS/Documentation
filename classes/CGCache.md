---
layout: default
title: CGCache
parent: Classes
has_children: false
has_toc: true
---

# CGCache
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Creates a new CCache instance.
# Constructor
```js
new CGCache(client, guild, options?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client instance. | false | *none* |
| guild | [Guild](/classes/Guild) | The guild instance. | false | *none* |
| options | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | true | *none* |

# Properties
## client
The client that initialized the cache.

**Type:** [Client](/classes/Client)

## guild
The guild instance this cache is for.

**Type:** [Guild](/classes/Guild)

# Methods
## array()
Get an array of the entries in the cache.

**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## arrayPair()
Get an array of the entries in the cache as `Pair`s.

**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## clear()
Clear the cache and its contents.

**Returns:** [Cache](/classes/Cache)

## entries()
Get an object of the entries in the cache. The
key is the key of the entry, and the value is
the value of the entry.

**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## filter(fn)
Filter values in the cache. If the key is not found
in the cache, an empty array is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## find(fn)
Find a value in the cache. If the key is not found
in the cache, `null` is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** any

## get(key)
Get a value from the cache. If the key is not found
in the cache, `null` is returned.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The key to get the value for. | false | *none* |

**Returns:** any

## has(key)
Check if the cache contains a key.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The key of the entry. | false | *none* |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

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
| key | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The key of the entry. | false | *none* |

**Returns:** [Cache](/classes/Cache)

## set(key, value, options?)
Set a value in the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The key of the entry. | false | *none* |
| value | any | The value to set it to. | false | *none* |
| options | any |   | true | *none* |

**Returns:** [Cache](/classes/Cache)

## size()
Get the amount of entries in the cache.

**Returns:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## strip(data)
A method called to strip unwanted properties from an
entry before it is added to the cache.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

