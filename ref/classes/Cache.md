---
layout: default
title: Cache
parent: Classes
has_children: false
has_toc: true
---

# Cache
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Cache(client)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |

# Properties
## client
**Type:** [Birb](/classes/Birb)

# Methods
## entries()
**Returns:** IterableIterator<*[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*>

## filter(fn)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## find(fn)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fn | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* |   | false | *none* |

**Returns:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| Pair<K, T>

## get(key)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | K |   | false | *none* |

**Returns:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| T

## has(key)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | K |   | false | *none* |

**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## keys()
**Returns:** IterableIterator<K>

## remove(key)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | K |   | false | *none* |

**Returns:** void

## set(key, value)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | K |   | false | *none* |
| value | T |   | false | *none* |

**Returns:** void

## size()
**Returns:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## take(key)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| key | K |   | false | *none* |

**Returns:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| T

## toArray()
**Returns:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## values()
**Returns:** IterableIterator<T>

