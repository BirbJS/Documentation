---
layout: default
title: MessageEmbed
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# MessageEmbed
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
The MessageEmbed class represents a message embed on
Discord. A message embed is a rich embed that can
include a lot of formatted data (they can also have
their color set which is quite nice).
# Constructor
```js
new MessageEmbed()
```

# Properties
## author
The author of this embed.

**Type:** [EmbedAuthor](/ref/classes/EmbedAuthor)

## color
The color of this embed as a hex string.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## description
The description of this embed.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## fields
This embed's fields.

**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## footer
The footer of this embed.

**Type:** [EmbedFooter](/ref/classes/EmbedFooter)

## image
The image in this embed.

**Type:** [EmbedMedia](/ref/classes/EmbedMedia)

## thumbnail
The thumbnail for this embed.

**Type:** [EmbedMedia](/ref/classes/EmbedMedia)

## timestamp
The timestamp of this embed (shows in the footer).

**Type:** Date

## title
The title of this embed.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## url
The URL of this embed (makes the title clickable).

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## video
The video for this embed (usually not settable).

**Type:** [EmbedMedia](/ref/classes/EmbedMedia)

# Methods
## addField(name, value, inline?)
Add a field to this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the field. | false | *none* |
| value | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The field's value. | false | *none* |
| inline | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* |   | true | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## addFields(fields)
Add multiple fields to this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fields | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The fields to add to this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## format()
Format this class into an API-acceptable object.

**Returns:** any

## removeField(index)
Remove a field from this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| index | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* | The array index of the field to remove. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setAuthor(name, url?, iconUrl?)
Set the author of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The name of the author. | false | *none* |
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |
| iconUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setColor(color)
Set the HEX color of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| color | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new HEX color of this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setDescription(description)
Set the description of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| description | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new description of this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setFields(fields)
Set the fields of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fields | *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)* | The new fields of this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setFooter(text, iconUrl?)
Set the footer of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| text | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The text of the footer. | false | *none* |
| iconUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setImage(url, height?, width?)
Set the image for this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | A public-facing URL to an image for the embed. | false | *none* |
| height | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |
| width | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setThumbnail(url, height?, width?)
Set the thumbnail for this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | A public-facing URL to an image for the embed. | false | *none* |
| height | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |
| width | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setTimestamp(timestamp)
Set the timestamp of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| timestamp | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* \| Date | The new timestamp of this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setTitle(title)
Set the title of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| title | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new title of this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setUrl(url)
Set the URL of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The new URL of this embed. | false | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

## setVideo(url, height?, width?)
Set the video for this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | A public-facing URL to a video for the embed. | false | *none* |
| height | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |
| width | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |

**Returns:** [MessageEmbed](/ref/classes/MessageEmbed)

