---
layout: default
title: InternalWebsocket
parent: Classes
grand_parent: Reference
has_children: false
has_toc: true
---

# InternalWebsocket
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
The InternalWebsocket class is a class that handles
the annoying stuff regarding websockets connected to
Discord (like compression and packing).
# Constructor
```js
new InternalWebsocket(client, domain)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/ref/classes/Client) | The client that owns this websocket. | false | *none* |
| domain | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* | The current Discord gateway URL.  | false | *none* |

# Properties
## buffer
{: .d-inline-block }

PROTECTED
{: .label .label-red }

The internal erlpack buffer.

**Type:** any

## client
The client that owns this websocket.

**Type:** [Client](/ref/classes/Client)

## domain
The current Discord gateway URL.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## encoding
The type of encoding to use. If `erlpack` is
installed (`npm install erlpack`), `etf` encoding
will be used. Otherwise, normal `json` encoding will
be used.

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## status
The current status of the websocket.

**Type:** [WebsocketStatus](/ref/enums/WebsocketStatus)

## url
The websocket's currently set URL.

**Type:** URL

# Methods
## generateURL()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Generates the gateway URL.

**Returns:** URL

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Initializes ZLib if supported.

**Returns:** void

## pack(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Packs data for sending to Discord. If the encoding
is set to `etf`, this method will use the
`zlib-sync` (`npm install zlib-sync`) library to
pack its `etf` data. Otherwise, parses the JSON data
to a string.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The data to pack. | false | *none* |

**Returns:** any

## processPacket(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Attempts to process a packet by using ZLib to let
Discord send packets in chunks. If ZLib is not yet
installed (`npm install zlib-sync`), this method
will just pass the data through for unpacking
(`this.unpack()`).

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The packet's data. | false | *none* |

**Returns:** any

## unpack(data, type?)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

Unpacks a packet using the current encoding. If the
encoding is set to `etf`, this method will use the
`zlib-sync` (`npm install zlib-sync`) library to
unpack its `etf` data. Otherwise, parses the data to
normal JSON.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any | The packet's data. | false | *none* |
| type | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** any

