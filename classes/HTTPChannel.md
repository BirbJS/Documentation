---
layout: default
title: HTTPChannel
parent: Classes
has_children: false
has_toc: true
---

# HTTPChannel
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new HTTPChannel()
```

# Methods
## addThreadMember(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| userId | string |   | false | *none* |

**Returns:** Promise<any>

## bulkDeleteMessages(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## createInvite(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## createMessage(client, channelId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

## createMessageReaction(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| emoji | string |   | false | *none* |

**Returns:** Promise<any>

## crossPostMessage(client, channelId, messageId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |

**Returns:** Promise<any>

## delete(client, channelId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## deleteAllMessageReactions(client, channelId, messageId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |

**Returns:** Promise<any>

## deleteAllMessageReactionsForEmoji(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| emoji | string |   | false | *none* |

**Returns:** Promise<any>

## deleteMessage(client, channelId, messageId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## deleteMessageReaction(client, channelId, messageId, userId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| userId | string |   | false | *none* |
| emoji | string |   | false | *none* |

**Returns:** Promise<any>

## deleteOwnMessageReaction(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| emoji | string |   | false | *none* |

**Returns:** Promise<any>

## deletePermission(client, channelId, overwriteId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| overwriteId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## dmAddRecipient(client, channelId, userId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| userId | string |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

## dmRemoveRecipient(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| userId | string |   | false | *none* |

**Returns:** Promise<any>

## editMessage(client, channelId, messageId, data, original?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| data | any |   | false | *none* |
| original | [Message](/classes/Message) |   | true | *none* |

**Returns:** Promise<any>

## editPermissions(client, channelId, overwriteId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| overwriteId | string |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

## followChannel(client, channelId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

## getInvites(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## getMessage(client, channelId, messageId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | any |   | false | *none* |

**Returns:** Promise<any>

## getMessageReactions(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | any |   | false | *none* |
| emoji | string |   | false | *none* |

**Returns:** Promise<any>

## getMessages(client, channelId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

## getPinnedMessages(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## getThreadMember(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| userId | string |   | false | *none* |

**Returns:** Promise<any>

## joinThread(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## leaveThread(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## listActiveThreads(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## listThreadMembers(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## modify(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## pinMessage(client, channelId, messageId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## removeThreadMember(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| userId | string |   | false | *none* |

**Returns:** Promise<any>

## startThreadWithMessage(client, channelId, messageId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## startThreadWithoutMessage(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## triggerTypingIndicator(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |

**Returns:** Promise<any>

## unpinMessage(client, channelId, messageId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| channelId | string |   | false | *none* |
| messageId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

