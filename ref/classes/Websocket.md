---
layout: default
title: Websocket
parent: Classes
has_children: false
has_toc: true
---

# Websocket
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Websocket(client, domain)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |
| domain | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

# Properties
## buffer
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Type:** any

## client
**Type:** [Birb](/classes/Birb)

## connectedSince
**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## doNotReconnect
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## domain
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## encoding
**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## expectedGuilds
**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## hasBeenReady
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## heartbeatInterval
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## lastHeartbeat
**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## lastHeartbeatAcked
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## lastResume
**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## lastSequenceIdentifier
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## ping
**Type:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

## resumeGatewayUrl
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## schedulerLoop
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| Timer

## sessionIdentifier
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## socket
**Type:** *[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)* \| WebSocket

## status
**Type:** [GatewayStatus](/enums/GatewayStatus)

## url
**Type:** URL

# Methods
## close(code?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| code | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* |   | true | *none* |

**Returns:** void

## connect()
**Returns:** void

## generateURL()
**Returns:** URL

## heartbeat()
**Returns:** Promise<void>

## init()
{: .d-inline-block }

PROTECTED
{: .label .label-red }

**Returns:** void

## isClosed()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isConnected()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## isConnecting()
**Returns:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## pack(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

## preventReconnect(value?)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| value | *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)* |   | true | *none* |

**Returns:** void

## processPacket(data)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |

**Returns:** any

## reconnect()
**Returns:** void

## send(data)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | Object |   | false | *none* |

**Returns:** void

## setSessionIdentifier(sessionIdentifier)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| sessionIdentifier | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | false | *none* |

**Returns:** void

## setStatus(status)
| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| status | [GatewayStatus](/enums/GatewayStatus) |   | false | *none* |

**Returns:** void

## terminate()
**Returns:** void

## unpack(data, type?)
{: .d-inline-block }

PROTECTED
{: .label .label-red }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| data | any |   | false | *none* |
| type | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* |   | true | *none* |

**Returns:** any

