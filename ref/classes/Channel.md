---
layout: default
title: Channel
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# Channel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
Represents any kind of channel on Discord.
# Constructor
```js
new Channel(client, data)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client this channel belongs to. | false | *none* |
| data | any | The data of this channel.  | false | *none* |

# Properties
## client
The client this channel belongs to.

**Type:** [Client](/ref/classes/Client)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

The ID of this channel.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## name
The name of this channel.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

# Methods
## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Initialize the data of this channel.

**Returns:** any

