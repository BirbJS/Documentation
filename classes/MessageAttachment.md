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
# Constructor
```js
new MessageAttachment(file, filename, id?, url?, proxyUrl?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
<<<<<<< Updated upstream
| file | Object | string | Buffer |  | false | null |
| filename | Object | string |  | false | null |
| id | string |  | true |  |
| url | string |  | true |  |
| proxyUrl | string |  | true |  |

# Properties
## buffer
**Type:** Object | Buffer
=======
| file | Object or string or Buffer | The file to upload. If a string, it is assumed to be the path to the file (which Birb.JS shall read and turn into a buffer). Rarely should be set to `null`. | false | null |
| filename | Object or string | The filename of the attachment. Rarely should be set to `null`. | false | null |
| id | string |   | true | *none* |
| url | string |   | true | *none* |
| proxyUrl | string |   | true | *none* |

# Properties
## buffer
The buffer containing this attachment's data.

**Type:** Object or Buffer
>>>>>>> Stashed changes

## filename
**Type:** string

## id
<<<<<<< Updated upstream
**Type:** Object | string

## proxyUrl
**Type:** Object | string

## url
**Type:** Object | string

# Methods
## getBuffer()
**Returns:** Object | Buffer
=======
The ID of this attachment. Not present if the
attachment is yet to be uploaded to Discord.

**Type:** Object or string

## proxyUrl
The Discord proxy URL to this attachment. Not
present if the attachment is yet to be uploaded to
Discord.

**Type:** Object or string

## url
The Discord CDN URL to this attachment. Not present
if the attachment is yet to be uploaded to Discord.

**Type:** Object or string

# Methods
## getBuffer()
Gets the attachment's data as a Buffer.

**Returns:** Object or Buffer
>>>>>>> Stashed changes

## fromApiMessage(attachments?)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| attachments | Object | Object |  | true |  |

**Returns:** Object

