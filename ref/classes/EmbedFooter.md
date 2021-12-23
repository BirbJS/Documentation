---
layout: default
title: EmbedFooter
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# EmbedFooter
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
An EmbedFooter stores data on the footer field of
a MessageEmbed.
# Constructor
```js
new EmbedFooter(text, iconUrl?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| text | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The text displayed at the bottom of the embed. | false | *none* |
| iconUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

# Properties
## iconUrl
The URL of the icon displayed at the bottom of the
embed.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## text
The text displayed at the bottom of the embed.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## format()
Format this class into an API-acceptable object.

**Returns:** any

## removeIcon()
Remove the the icon displayed at the bottom of the
embed.

**Returns:** [EmbedFooter](/ref/classes/EmbedFooter)

## setIconUrl(iconUrl?)
Set the URL of the icon displayed at the bottom of the
embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| iconUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** [EmbedFooter](/ref/classes/EmbedFooter)

## setText(text)
Set the text displayed at the bottom of the embed.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| text | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The text displayed at the bottom of the embed. | false | *none* |

**Returns:** [EmbedFooter](/ref/classes/EmbedFooter)

