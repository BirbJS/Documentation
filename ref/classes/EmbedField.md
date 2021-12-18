---
layout: default
title: EmbedField
parent: Classes
grand_parent: Reference
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
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the field. | false | *none* |
| value | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The value of the field. | false | *none* |
| inline | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* |   | true | *none* |

# Properties
## inline
Whether or not this field is inline.

**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## name
The name of the field.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## value
The value of the field.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** any

## setInline(inline)
Set whether or not this field is inline.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| inline | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* | Whether or not this field is inline. | false | *none* |

**Returns:** [EmbedField](/ref/classes/EmbedField)

## setName(name)
Set the name of the field.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the field. | false | *none* |

**Returns:** [EmbedField](/ref/classes/EmbedField)

## setValue(value)
Set the value of the field.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| value | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The value of the field. | false | *none* |

**Returns:** [EmbedField](/ref/classes/EmbedField)

