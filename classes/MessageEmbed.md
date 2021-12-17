---
layout: default
title: MessageEmbed
parent: Classes
has_children: false
has_toc: true
---

# MessageEmbed
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
## Constructor
```js
new MessageEmbed()
```
## Properties
### author
**Type:** Object | [EmbedAuthor](classes/EmbedAuthor)

### color
**Type:** Object | string

### description
**Type:** Object | string

### fields
**Type:** Object

### footer
**Type:** Object | [EmbedFooter](classes/EmbedFooter)

### image
**Type:** Object | [EmbedMedia](classes/EmbedMedia)

### thumbnail
**Type:** Object | [EmbedMedia](classes/EmbedMedia)

### timestamp
**Type:** Object | Date

### title
**Type:** Object | string

### url
**Type:** Object | string

### video
**Type:** Object | [EmbedMedia](classes/EmbedMedia)

## Methods
### addField(name, value, inline?)
Add a field to this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name of the field. | false |  |
| value | string | The field's value. | false |  |
| inline | boolean |  | true |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### addFields(fields)
Add multiple fields to this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fields | Object | The fields to add to this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### format()
Format this class into an API-acceptable object.

**Returns:** Object

### removeField(index)
Remove a field from this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| index | number | The array index of the field to remove. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setAuthor(name, url?, iconUrl?)
Set the author of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name of the author. | false |  |
| url | string |  | true |  |
| iconUrl | string |  | true |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setColor(color)
Set the HEX color of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| color | string | The new HEX color of this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setDescription(description)
Set the description of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| description | string | The new description of this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setFields(fields)
Set the fields of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| fields | Object | The new fields of this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setFooter(text, iconUrl?)
Set the footer of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| text | string | The text of the footer. | false |  |
| iconUrl | string |  | true |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setImage(url, height?, width?)
Set the image for this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | string | A public-facing URL to an image for the embed. | false |  |
| height | number |  | true |  |
| width | number |  | true |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setThumbnail(url, height?, width?)
Set the thumbnail for this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | string | A public-facing URL to an image for the embed. | false |  |
| height | number |  | true |  |
| width | number |  | true |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setTimestamp(timestamp)
Set the timestamp of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| timestamp | number | Date | The new timestamp of this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setTitle(title)
Set the title of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| title | string | The new title of this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setUrl(url)
Set the URL of this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | string | The new URL of this embed. | false |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

### setVideo(url, height?, width?)
Set the video for this embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | string | A public-facing URL to a video for the embed. | false |  |
| height | number |  | true |  |
| width | number |  | true |  |

**Returns:** [MessageEmbed](classes/MessageEmbed)

