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
| file | Object | string | Buffer |  | false | null |
| filename | Object | string |  | false | null |
| id | string |  | true |  |
| url | string |  | true |  |
| proxyUrl | string |  | true |  |

# Properties
## buffer
**Type:** Object | Buffer

## filename
**Type:** string

## id
**Type:** Object | string

## proxyUrl
**Type:** Object | string

## url
**Type:** Object | string

# Methods
## getBuffer()
**Returns:** Object | Buffer

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

