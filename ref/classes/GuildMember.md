---
layout: default
title: GuildMember
parent: Classes
has_children: false
has_toc: true
---

# GuildMember
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new GuildMember(client, guild, member)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| client | [Birb](/classes/Birb) |   | false | *none* |
| guild | [Guild](/classes/Guild) |   | false | *none* |
| member | APIGuildMemberWithUser |   | false | *none* |

# Properties
## avatarHash
**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## client
**Type:** [Birb](/classes/Birb)

## guild
**Type:** [Guild](/classes/Guild)

## id
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## joinedAt
{: .d-inline-block }

READONLY
{: .label .label-purple }

**Type:** Date

## nickname
**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)*

## nitroBoostingSince
**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| Date

## pendingMembershipScreening
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## roles
**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

## timedOutUntil
**Type:** *[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)* \| Date

## user
**Type:** [User](/classes/User)

## voiceDeafened
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

## voiceMuted
**Type:** *[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean)*

