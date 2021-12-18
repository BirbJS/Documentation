---
layout: default
title: Channel
parent: Classes
has_children: false
has_toc: true
---

# Channel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
A Channel represents any channel on Discord.
# Constructor
```js
new Channel(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) | The client this channel belongs to. | false | *none* |
| data | any | The data of this channel.
 | false | *none* |

# Properties
## client
The client this channel belongs to.

**Type:** [Client](/classes/Client)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this channel.

**Type:** string

## name
The name of this channel.

**Type:** string

# Methods
## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Initialize the data of this channel.

**Returns:** any

