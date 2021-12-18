---
layout: default
title: EmbedMedia
parent: Classes
has_children: false
has_toc: true
---

# EmbedMedia
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
An EmbedMedia stores data on a media or attachment
field of a MessageEmbed.
# Constructor
```js
new EmbedMedia(url, height?, width?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The URL of the media. If refrences an attachment, prefix with `attachment://` followed by the attachment's filename. | false | *none* |
| height | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |
| width | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |

# Properties
## height
The height of the media.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## url
The URL of the media.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## width
The width of the media.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** any

## removeHeight()
Remove the height of the media.

**Returns:** [EmbedMedia](/classes/EmbedMedia)

## removeWidth()
Remove the width of the media.

**Returns:** [EmbedMedia](/classes/EmbedMedia)

## setHeight(height)
Set the height of the media.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| height | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The height of the media. `null` to remove the height. | false | *none* |

**Returns:** [EmbedMedia](/classes/EmbedMedia)

## setUrl(url)
Set the URL of the media.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The URL of the media. If refrences an attachment, prefix with `attachment://` followed by the attachment's filename. | false | *none* |

**Returns:** [EmbedMedia](/classes/EmbedMedia)

## setWidth(width)
Set the width of the media.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| width | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The width of the media. `null` to remove the width. | false | *none* |

**Returns:** [EmbedMedia](/classes/EmbedMedia)

