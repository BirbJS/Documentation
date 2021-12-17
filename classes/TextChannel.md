---
layout: default
title: TextChannel
parent: Classes
has_children: false
has_toc: true
---

# TextChannel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new TextChannel(client, data, options?, guild?)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |  | false |  |
| data | any |  | false |  |
| options | Object |  | true |  |
| guild | [Guild](/classes/Guild) |  | true |  |

# Properties
## client
**Type:** [Client](/classes/Client)

## guild
**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** string

## messages
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** [MessageBlock](/classes/MessageBlock)

## name
**Type:** string

## permissions
**Type:** [ChannelPermissionsBlock](/classes/ChannelPermissionsBlock)

# Methods
## build(data)
{: .d-inline-block }

PRIVATE
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |

**Returns:** void

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** undefined | [TextChannel](/classes/TextChannel)

## modify(data, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## send(message)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| message | MessageContent |  | false |  |

**Returns:** Promise<[Message](/classes/Message)>

## set()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Set the TextChannel's data to the cache.

**Returns:** [TextChannel](/classes/TextChannel)

## setAutoArchive(minutes, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| minutes | number |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setNSFW(nsfw, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| nsfw | boolean |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setName(name, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| name | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setOverwrites(overwrite)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| overwrite | Object |  | false |  |

**Returns:** Promise<void>

## setPosition(position, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| position | number |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setSlowmode(seconds, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| seconds | number |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

## setTopic(topic, reason?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| topic | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<[TextChannel](/classes/TextChannel)>

