---
layout: default
title: EmbedAuthor
parent: Classes
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
| name | string | The name of the author. | false | *none* |
| url | string |   | true | *none* |
| iconUrl | string |   | true | *none* |

# Properties
## iconUrl
The icon URL of the author.

**Type:** Object | string

## name
The name of the author.

**Type:** string

## url
The URL of the author.

**Type:** Object | string

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** any

## removeIcon()
Remove the author's icon.

**Returns:** [EmbedAuthor](/classes/EmbedAuthor)

## removeUrl()
Remove the author's URL.

**Returns:** [EmbedAuthor](/classes/EmbedAuthor)

## setIconUrl(iconUrl)
Set the icon URL of the author.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| iconUrl | Object | string | A publicly-accessible URL to an image to use as the author's icon. `null` to remove the icon. | false | *none* |

**Returns:** [EmbedAuthor](/classes/EmbedAuthor)

## setName(name)
Set the name of the author.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string | The name of the author. | false | *none* |

**Returns:** [EmbedAuthor](/classes/EmbedAuthor)

## setUrl(url)
Set the URL of the author.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| url | Object | string | The URL of the author. `null` to remove the URL. | false | *none* |

**Returns:** [EmbedAuthor](/classes/EmbedAuthor)

