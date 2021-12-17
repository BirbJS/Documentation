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
## Constructor
```js
new HTTPChannel()
```
## Methods
### addThreadMember(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

### bulkDeleteMessages(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### createInvite(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### createMessage(client, channelId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

### createMessageReaction(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| emoji | string |  | false |  |

**Returns:** Promise<any>

### crossPostMessage(client, channelId, messageId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |

**Returns:** Promise<any>

### delete(client, channelId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### deleteAllMessageReactions(client, channelId, messageId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |

**Returns:** Promise<any>

### deleteAllMessageReactionsForEmoji(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| emoji | string |  | false |  |

**Returns:** Promise<any>

### deleteMessage(client, channelId, messageId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### deleteMessageReaction(client, channelId, messageId, userId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| userId | string |  | false |  |
| emoji | string |  | false |  |

**Returns:** Promise<any>

### deleteOwnMessageReaction(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| emoji | string |  | false |  |

**Returns:** Promise<any>

### deletePermission(client, channelId, overwriteId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| overwriteId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### dmAddRecipient(client, channelId, userId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| userId | string |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

### dmRemoveRecipient(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

### editMessage(client, channelId, messageId, data, original?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| data | any |  | false |  |
| original | [Message](classes/Message) |  | true |  |

**Returns:** Promise<any>

### editPermissions(client, channelId, overwriteId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| overwriteId | string |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

### followChannel(client, channelId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

### getInvites(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### getMessage(client, channelId, messageId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | any |  | false |  |

**Returns:** Promise<any>

### getMessageReactions(client, channelId, messageId, emoji)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | any |  | false |  |
| emoji | string |  | false |  |

**Returns:** Promise<any>

### getMessages(client, channelId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

### getPinnedMessages(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### getThreadMember(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

### joinThread(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### leaveThread(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### listActiveThreads(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### listThreadMembers(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### modify(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### pinMessage(client, channelId, messageId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### removeThreadMember(client, channelId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

### startThreadWithMessage(client, channelId, messageId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### startThreadWithoutMessage(client, channelId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### triggerTypingIndicator(client, channelId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |

**Returns:** Promise<any>

### unpinMessage(client, channelId, messageId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| channelId | string |  | false |  |
| messageId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

