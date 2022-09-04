---
layout: default
title: EventListener
parent: Classes
has_children: false
has_toc: true
---

# EventListener
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new EventListener(parent, event)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| parent | EventDispatcher<E> |   | false | *none* |
| event | E |   | false | *none* |

# Methods
## do(handler)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| handler | F |   | false | *none* |

**Returns:** EventListener<E, F>

## forget()
**Returns:** void

## once()
**Returns:** EventListener<E, F>

