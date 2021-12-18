---
layout: default
title: EmbedField
parent: Classes
has_children: false
has_toc: true
---

# EmbedField
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
An EmbedField stores data on a field of a
MessageEmbed.
# Constructor
```js
new EmbedField(name, value, inline?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name of the field. | false | *none* |
| value | string | The value of the field. | false | *none* |
| inline | boolean |   | true | *none* |

# Properties
## inline
Whether or not this field is inline.

**Type:** boolean

## name
The name of the field.

**Type:** string

## value
The value of the field.

**Type:** string

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** any

## setInline(inline)
Set whether or not this field is inline.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| inline | boolean | Whether or not this field is inline. | false | *none* |

**Returns:** [EmbedField](/classes/EmbedField)

## setName(name)
Set the name of the field.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name of the field. | false | *none* |

**Returns:** [EmbedField](/classes/EmbedField)

## setValue(value)
Set the value of the field.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| value | string | The value of the field. | false | *none* |

**Returns:** [EmbedField](/classes/EmbedField)

