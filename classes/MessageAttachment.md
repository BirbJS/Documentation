---
layout: default
title: MessageAttachment
parent: Classes
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
| file | Object | string | Buffer | The file to upload. If a string, it is assumed to be the path to the file (which Birb.JS shall read and turn into a buffer). Rarely should be set to `null`. | false | null |
| filename | Object | string | The filename of the attachment. Rarely should be set to `null`. | false | null |
| id | string |   | true | *none* |
| url | string |   | true | *none* |
| proxyUrl | string |   | true | *none* |

# Properties
## buffer
The buffer containing this attachment's data.

**Type:** Object | Buffer

## filename
The filename of this attachment. Can be used to
represent this attachment in embededs. For example,
if the filename is `image.png`, then the attachment
URL would be `attachment://image.png`.

**Type:** string

## id
The ID of this attachment. Not present if the
attachment is yet to be uploaded to Discord.

**Type:** Object | string

## proxyUrl
The Discord proxy URL to this attachment. Not
present if the attachment is yet to be uploaded to
Discord.

**Type:** Object | string

## url
The Discord CDN URL to this attachment. Not present
if the attachment is yet to be uploaded to Discord.

**Type:** Object | string

# Methods
## getBuffer()
Gets the attachment's data as a Buffer.

**Returns:** Object | Buffer

