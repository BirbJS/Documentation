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
# Constructor
```js
new EmbedAuthor(name, url?, iconUrl?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string |  | false |  |
| url | string |  | true |  |
| iconUrl | string |  | true |  |

# Properties
## iconUrl
<<<<<<< Updated upstream
**Type:** Object | string
=======
The icon URL of the author.

**Type:** Object or string
>>>>>>> Stashed changes

## name
**Type:** string

## url
<<<<<<< Updated upstream
**Type:** Object | string
=======
The URL of the author.

**Type:** Object or string
>>>>>>> Stashed changes

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** Object

## removeIcon()
**Returns:** void

## removeUrl()
**Returns:** void

## setIconUrl(iconUrl)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
<<<<<<< Updated upstream
| iconUrl | string |  | false |  |
=======
| iconUrl | Object or string | A publicly-accessible URL to an image to use as the author's icon. `null` to remove the icon. | false | *none* |
>>>>>>> Stashed changes

**Returns:** void

## setName(name)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string |  | false |  |

**Returns:** void

## setUrl(url)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
<<<<<<< Updated upstream
| url | string |  | false |  |
=======
| url | Object or string | The URL of the author. `null` to remove the URL. | false | *none* |
>>>>>>> Stashed changes

**Returns:** void

