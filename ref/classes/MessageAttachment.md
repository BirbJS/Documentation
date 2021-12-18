---
layout: default
title: MessageAttachment
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# MessageAttachment
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Creates a new attachment. Does not upload the
attachment to Discord.
# Constructor
```js
new MessageAttachment(file, filename, id?, url?, proxyUrl?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| file | *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* \| Buffer | The file to upload. If a string, it is assumed to be the path to the file (which Birb.JS shall read and turn into a buffer). Rarely should be set to `null`. | false | null |
| filename | *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The filename of the attachment. Rarely should be set to `null`. | false | null |
| id | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |
| url | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |
| proxyUrl | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

# Properties
## buffer
The buffer containing this attachment's data.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| Buffer

## filename
The filename of this attachment. Can be used to
represent this attachment in embededs. For example,
if the filename is `image.png`, then the attachment
URL would be `attachment://image.png`.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## id
The ID of this attachment. Not present if the
attachment is yet to be uploaded to Discord.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## proxyUrl
The Discord proxy URL to this attachment. Not
present if the attachment is yet to be uploaded to
Discord.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## url
The Discord CDN URL to this attachment. Not present
if the attachment is yet to be uploaded to Discord.

**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## getBuffer()
Gets the attachment's data as a Buffer.

**Returns:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| Buffer

