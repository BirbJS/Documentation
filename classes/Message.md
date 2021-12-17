---
layout: default
title: Message
parent: Classes
has_children: false
has_toc: true
---

# Message
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Message(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |

# Properties
## attachments
**Type:** Object

## author
**Type:** Object | [BaseUser](/classes/BaseUser)

## baseAuthor
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Type:** any

## channel
**Type:** [TextBasedChannel](/classes/TextBasedChannel)

## client
**Type:** [Client](/classes/Client)

## content
**Type:** Object | string

## flags
**Type:** number

## guild
**Type:** Object | [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## member
**Type:** Object | [GuildMember](/classes/GuildMember)

## system
**Type:** boolean

## type
**Type:** Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object | Object

## webhookId
**Type:** Object | string

# Methods
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## crosspost()
**Returns:** Promise<[Message](/classes/Message)>

## delete()
**Returns:** Promise<void>

## edit(message)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## modify(data)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## parse(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## pin(reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | string |  | true |  |

**Returns:** Promise<[Message](/classes/Message)>

## reply(message)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## set()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Returns:** [Message](/classes/Message)

## startThread(name, options)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string |  | false |  |
| options | Object |  | false | {} |

**Returns:** Promise<void>

## supressEmbeds()
**Returns:** Promise<[Message](/classes/Message)>

## unpin(reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| reason | string |  | true |  |

**Returns:** Promise<[Message](/classes/Message)>

## waitForAuthor()
{: .d-inline-block }

PRIVATE
{: .label .label-red }

**Returns:** Promise<[Message](/classes/Message)>

## buildApiMessage(data, edit)
{: .d-inline-block }

STATIC
{: .label .label-blue }
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | MessageContent |  | false |  |
| edit | boolean |  | false | false |

**Returns:** any

