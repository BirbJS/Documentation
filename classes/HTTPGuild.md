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
# Constructor
```js
new HTTPGuild()
```

# Methods
## addMember(client, guildId, userId, data)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| data | any |   | false | *none* |

**Returns:** Promise<any>

## addMemberRole(client, guildId, userId, roleId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| roleId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## beginPrune(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## createBan(client, guildId, userId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## createChannel(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## createRole(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## delete(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## deleteIntegration(client, guildId, integrationId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| integrationId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## deleteRole(client, guildId, roleId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| roleId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## get(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getActiveThreads(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getBan(client, guildId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |

**Returns:** Promise<any>

## getBans(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getChannels(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getIntegrations(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getInvites(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getMember(client, guildId, userId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |

**Returns:** Promise<any>

## getMembers(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getPreview(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getPruneCount(client, guildId, days, includeRoles?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| days | number |   | false | *none* |
| includeRoles | string |   | true | *none* |

**Returns:** Promise<any>

## getRoles(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getVanityUrl(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getVoiceRegions(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getWelcomeScreen(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getWidget(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## getWidgetSettings(client, guildId)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |

**Returns:** Promise<any>

## modify(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyChannelPositions(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyCurrentMember(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyMember(client, guildId, userId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyRole(client, guildId, roleId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| roleId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyRolePositions(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyVoiceState(client, guildId, userId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyWelcomeScreen(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## modifyWidget(client, guildId, data, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| data | any |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## removeBan(client, guildId, userId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## removeMember(client, guildId, userId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## removeMemberRole(client, guildId, userId, roleId, reason?)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| userId | string |   | false | *none* |
| roleId | string |   | false | *none* |
| reason | string |   | true | *none* |

**Returns:** Promise<any>

## searchMembers(client, guildId, query)
{: .d-inline-block }

STATIC
{: .label .label-blue }

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Client](/classes/Client) |   | false | *none* |
| guildId | string |   | false | *none* |
| query | string |   | false | *none* |

**Returns:** Promise<any>

