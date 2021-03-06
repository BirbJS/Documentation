---
layout: default
title: EmbedAuthor
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# EmbedAuthor
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
An EmbedAuthor stores data on the author field of
MessageEmbeds.
# Constructor
```js
new EmbedAuthor(name, url?, iconUrl?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the author. | false | *none* |
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |
| iconUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

# Properties
## iconUrl
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## name
The name of the author.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## url
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** any

## removeIcon()
Remove the author's icon.

**Returns:** [EmbedAuthor](/ref/classes/EmbedAuthor)

## removeUrl()
Remove the author's URL.

**Returns:** [EmbedAuthor](/ref/classes/EmbedAuthor)

## setIconUrl(iconUrl?)
Set the icon URL of the author.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| iconUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | A publicly-accessible URL to an image to use as the author's icon. Pass through no arguments to remove the icon. | true | *none* |

**Returns:** [EmbedAuthor](/ref/classes/EmbedAuthor)

## setName(name)
Set the name of the author.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the author. | false | *none* |

**Returns:** [EmbedAuthor](/ref/classes/EmbedAuthor)

## setUrl(url?)
Set the URL of the author.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The URL of the author. Pass through no arguments to remove the URL. | true | *none* |

**Returns:** [EmbedAuthor](/ref/classes/EmbedAuthor)

