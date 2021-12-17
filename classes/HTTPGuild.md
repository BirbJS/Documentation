---
layout: default
title: HTTPGuild
parent: Classes
has_children: false
has_toc: true
---

# HTTPGuild
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
## Constructor
```js
new HTTPGuild()
```
## Methods
### addMember(client, guildId, userId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| data | any |  | false |  |

**Returns:** Promise<any>

### addMemberRole(client, guildId, userId, roleId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| roleId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### beginPrune(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### createBan(client, guildId, userId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### createChannel(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### createRole(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### delete(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### deleteIntegration(client, guildId, integrationId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| integrationId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### deleteRole(client, guildId, roleId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| roleId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### get(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getActiveThreads(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getBan(client, guildId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

### getBans(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getChannels(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getIntegrations(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getInvites(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getMember(client, guildId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |

**Returns:** Promise<any>

### getMembers(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getPreview(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getPruneCount(client, guildId, days, includeRoles?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| days | number |  | false |  |
| includeRoles | string |  | true |  |

**Returns:** Promise<any>

### getRoles(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getVanityUrl(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getVoiceRegions(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getWelcomeScreen(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getWidget(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### getWidgetSettings(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |

**Returns:** Promise<any>

### modify(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyChannelPositions(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyCurrentMember(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyMember(client, guildId, userId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyRole(client, guildId, roleId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| roleId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyRolePositions(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyVoiceState(client, guildId, userId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyWelcomeScreen(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### modifyWidget(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| data | any |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### removeBan(client, guildId, userId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### removeMember(client, guildId, userId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### removeMemberRole(client, guildId, userId, roleId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| userId | string |  | false |  |
| roleId | string |  | false |  |
| reason | string |  | true |  |

**Returns:** Promise<any>

### searchMembers(client, guildId, query)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](classes/Client) |  | false |  |
| guildId | string |  | false |  |
| query | string |  | false |  |

**Returns:** Promise<any>

