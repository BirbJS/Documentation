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

| name | type | description | default |
|:-----|:-----|:------------|:--------|
| parent | EventDispatcher<E> |   | *none* |
| event | E |   | *none* |

# Methods
## do(handler)
| name | type | description | default |
|:-----|:-----|:------------|:--------|
| handler | F |   | *none* |

**Returns:** EventListener<E, F>

## forget()
**Returns:** void

## once()
**Returns:** EventListener<E, F>

